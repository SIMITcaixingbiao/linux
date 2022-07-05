### 1.进入根目录
```shell
[root@localhost ~]# cd /
[root@localhost /]# 
```
### 2.新建一个文件夹wulin
```shell
[root@localhost /]# mkdir wulin
[root@localhost /]# ls
aa  bin  boot  china  cs  dev  etc  home  hunan  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var  wulin
[root@localhost /]# 
```
### 3.进入武汉，然后新建三个文件夹 huashan shaolin mingjiao 
```shell
[root@localhost /]# cd wulin
[root@localhost wulin]# mkdir huashan shaolin mingjiao
[root@localhost wulin]# ls
huashan  mingjiao  shaolin
[root@localhost wulin]# 
```
### 4.进入mingjiao，新建三个文件夹 zhangwuji zhaomin xiaozhao
```shell
[root@localhost wulin]# cd mingjiao
[root@localhost mingjiao]# mkdir zhangwuji zhaomin xiaozhao
[root@localhost mingjiao]# ls
xiaozhao  zhangwuji  zhaomin
[root@localhost mingjiao]# 
```
### 5.进入zhangwuji文件夹，显示当前位置
```shell
[root@localhost mingjiao]# cd zhangwuji
[root@localhost zhangwuji]# pwd
/wulin/mingjiao/zhangwuji
[root@localhost zhangwuji]# 

```
### 6.返回到wulin文件夹
```shell
[root@localhost zhangwuji]# cd /wulin
[root@localhost wulin]# 

```
### 7.显示wulin的目录结构
```shell
[root@localhost wulin]# tree /wulin
/wulin
├── huashan
├── mingjiao
│   ├── xiaozhao
│   ├── zhangwuji
│   └── zhaomin
└── shaolin

6 directories, 0 files
[root@localhost wulin]# 

```
### 8.查找ip地址
```shell
[root@localhost wulin]# ip add
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host 
       valid_lft forever preferred_lft forever
2: ens33: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
    link/ether 00:0c:29:7d:13:c0 brd ff:ff:ff:ff:ff:ff
    inet 192.168.40.128/24 brd 192.168.40.255 scope global noprefixroute dynamic ens33
       valid_lft 1291sec preferred_lft 1291sec
    inet6 fe80::b70c:7914:2f8b:3378/64 scope link noprefixroute 
       valid_lft forever preferred_lft forever
[root@localhost wulin]# 

```
### 9.安装vim软件
```shell
[root@localhost wulin]# yum install vim -y
已加载插件：fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirrors.cn99.com
 * extras: mirrors.cn99.com
 * updates: mirrors.cn99.com
base                                                                                                                                                                                        | 3.6 kB  00:00:00     
extras                                                                                                                                                                                      | 2.9 kB  00:00:00     
updates                                                                                                                                                                                     | 2.9 kB  00:00:00     
updates/7/x86_64/primary_db                                                                                                                                                                 |  16 MB  00:00:04     
软件包 2:vim-enhanced-7.4.629-8.el7_9.x86_64 已安装并且是最新版本
无须任何处理
[root@localhost wulin]# 

```
