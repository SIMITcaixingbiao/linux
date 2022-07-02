### 1.查看当前linux系统里有哪些shell
```shell
[root@localhost ~]# cat /etc/shells
/bin/sh
/bin/bash
/usr/bin/sh
/usr/bin/bash
[root@localhost ~]# 
```
### 2.查看当前linux系统默认的shell
```shell
[root@localhost ~]# echo $SHELL
/bin/bash
[root@localhost ~]# 
```
### 3.切换下sh与bash
```shell
[root@localhost ~]# sh
sh-4.2# bash
[root@scliu ~]# 
```
### 4.使用which查寻ip命令的路径
```shell
[root@scliu ~]# which ip
/sbin/ip

```
### 5.查询ip命令是通过那个软件安装的
```shell
[root@scliu ~]# which ip
/sbin/ip
[root@scliu ~]# rpm -qf /usr/sbin/ip
iproute-4.11.0-30.el7.x86_64
[root@scliu ~]# yum provides ip
已加载插件：fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirrors.aliyun.com
 * extras: mirrors.aliyun.com
 * updates: mirrors.aliyun.com
updates/7/x86_64/filelists_db                                                                                                                                                               | 9.1 MB  00:00:02     
iproute-4.11.0-30.el7.x86_64 : Advanced IP routing and network device configuration tools
源    ：base
匹配来源：
文件名    ：/sbin/ip



iproute-4.11.0-30.el7.x86_64 : Advanced IP routing and network device configuration tools
源    ：base
匹配来源：
文件名    ：/usr/sbin/ip



iproute-4.11.0-30.el7.x86_64 : Advanced IP routing and network device configuration tools
源    ：@anaconda
匹配来源：
文件名    ：/sbin/ip



iproute-4.11.0-30.el7.x86_64 : Advanced IP routing and network device configuration tools
源    ：@anaconda
匹配来源：
文件名    ：/usr/sbin/ip


```
### 6.查询netstat是通过哪个软件安装过来的
```shell
[root@scliu ~]# yum provides netstat
已加载插件：fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirror.lzu.edu.cn
 * extras: ftp.sjtu.edu.cn
 * updates: ftp.sjtu.edu.cn
net-tools-2.0-0.25.20131004git.el7.x86_64 : Basic networking tools
源    ：base
匹配来源：
文件名    ：/bin/netstat



net-tools-2.0-0.25.20131004git.el7.x86_64 : Basic networking tools
源    ：@base
匹配来源：
文件名    ：/bin/netstat



net-tools-2.0-0.25.20131004git.el7.x86_64 : Basic networking tools
源    ：@base
匹配来源：
文件名    ：/usr/bin/netstat


```
### 7.安装netatat命令对应的安装包
```shell
[root@scliu ~]# yum install net-tools -y
已加载插件：fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirrors.njupt.edu.cn
 * extras: ftp.sjtu.edu.cn
 * updates: ftp.sjtu.edu.cn
软件包 net-tools-2.0-0.25.20131004git.el7.x86_64 已安装并且是最新版本
无须任何处理

```
### 8.新建结构为/hunan/changsha/nongda/sanchuang/feng的文件夹
```shell
[root@scliu ~]# mkdir -p /hunan/changsha/nongda/sanchuang/feng

```
### 9.查看/hunan文件夹的结构目录
```shell
[root@scliu ~]# tree /hunan
/hunan
└── changsha
    └── nongda
        └── sanchuang
            ├── fen
            └── feng

5 directories, 0 files

```
### 10.新建用户zhangjian
```shell
[root@scliu ~]# useradd zhangjian

```
### 11.进入zhangjian用户的家目录
```shell
[root@scliu ~]# cd ~zhangjian

```
### 12.返回上一级目录
```shell
[root@scliu zhangjian]# cd ..

```
### 13.进入当前用户的家目录
```shell
[root@scliu zhangjian]# cd
[root@scliu ~]# 

```
### 14.返回到上一次所在目录
```shell
[root@scliu home]# cd -
/home/zhangjian

```
### 15.切换zhangjian登录系统
```shell
[root@scliu zhangjian]# su - zhangjian

```
### 16.在当前用户文件夹下新建文件夹.nongda
```shell
[zhangjian@scliu ~]$ mkdir .nongda

```
### 17.显示当前所有文件夹
```shell
[zhangjian@scliu ~]$ ll
总用量 0
drwxrwxr-x. 2 zhangjian zhangjian 6 6月  29 21:22 nongda
[zhangjian@scliu ~]$ ls -a
.  ..  .bash_history  .bash_logout  .bash_profile  .bashrc  nongda  .nongda

```
### 18.退出当前用户
```shell
[zhangjian@scliu ~]$ exit
登出

```
### 19.查看pwd的操作手册
```shell
[root@scliu zhangjian]# man pwd

```

