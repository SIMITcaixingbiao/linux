### 1.新建用户bangyou
```shell
[root@localhost wulin]# useradd bangyou
useradd：用户“bangyou”已存在

```
### 2.切换用户到bangyou登录linux
```shell
[root@localhost wulin]# su - bangyou
上一次登录：二 6月 28 10:42:27 CST 2022pts/0 上

```
### 3.显示当前所在路径
```shell
[bangyou@localhost ~]$ pwd
/home/bangyou

```
### 4.在bangyou的家目录下新建文件夹sanchuang
```shell
[bangyou@localhost ~]$ mkdir sanchuang
[bangyou@localhost ~]$ ls
canxhuang  sanchuang

```
### 5.查看主机名
```shell
[bangyou@localhost ~]$ hostname
localhost.localdomain

```
### 6.退出bangyou用户
```shell
[bangyou@localhost ~]$ exit
登出

```
### 7.修改主机名为hunan-wangzhe-5
```shell
[root@localhost wulin]# hostname hunan-wangzhe-5
```
### 8.切换用户到bangyou登录linux，查看主机名提示符有无变化
```shell

[root@localhost wulin]# su - bangyou
上一次登录：六 7月  2 13:17:16 CST 2022pts/0 上
[bangyou@hunan-wangzhe-5 ~]$ hostnamectl set-hostname localhost

```
