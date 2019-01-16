---
layout: post
title:  "Linux ls 的长格式的命令输出"
---

# Linux ls 的长格式的命令输出

- 使用 `ls -l` 可以以长格式显示 Linux 对应目录下的文件信息

例:

`-rw-rw-r-- 1 ubuntu ubuntu 3916 Oct 18 22:21 index.html`

| 内容 | 描述 |
| --- | --- |
| `-rw-rw-r--` | 文件权限 |
| `1` | 链接数，文件夹因为内部需要以 `.` 链接到自身，因此至少为2 |
| `ubuntu` | 所属用户 |
| `ubuntu` | 所属用户组 |
| `3916` | 文件大小 |
| `Oct 18 22:21` | 最后修改时间 |
| `index.html` | 文件名 |
