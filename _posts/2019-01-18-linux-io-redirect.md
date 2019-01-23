---
layout: post
title:  "Linux IO 重定向"
categories: [linux]
tags: [linux]
---

## 文件流种类

| 编号 | 种类 |
| --- | --- |
| 0 | 标准输入 |
| 1 | 标准输出 |
| 2 | 标准错误 |

## 标准输出

### 覆写文件
```` bash
ls . > output.txt 
````

### 追加内容

```` bash
ls . >> output.txt
````

## 标准错误

### 重定向标准错误
```` bash
ls /not_exist_dir 2> error.txt
````
### 重定向标准输出及标准错误

#### 较旧版本也可支持
```` bash
ls /some_dir > output.txt 2>&1
````
#### 新版本
```` bash
ls /some_dir &> output.txt
````

## 不输出内容

```` bash
ls /some_dir &> /dev/null
````

## 标准输入

```` bash
cat < import.txt
````