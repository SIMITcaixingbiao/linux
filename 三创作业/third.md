### 1.查看主机名
```shell
[root@localhost ~]# hostname
localhost

```
### 2.查看第一提示符的值
```shell
[root@localhost ~]# echo $PS1
[\u@\h \W]\$

```
### 3.新建一个用户liuyi
```shell
[root@localhost ~]# useradd liuyi

```
### 4.修改主机名为scliu
```shell
[root@localhost ~]# hostname scliu

```
### 5.切换用户到liuyi
```shell
[root@localhost ~]# su - liuyi
[liuyi@scliu ~]$ 
```
### 6.观察一下主机名与用户名的变化
```shell

```
### 7.定义一个变量big_city赋值changsha
```shell
[liuyi@scliu ~]$ big_city='changsha'

```
### 8.新建一个文件夹引用big_city的值
```shell
[liuyi@scliu ~]$ mkdir $big_city
[liuyi@scliu ~]$ ls
changsha

```
### 9.修改第一提示符为'\u@\h:\t:\$'
```shell
[liuyi@scliu ~]$ PS1='\u@\h:\t:\$'

```
### 10.修改第二提示符为'>>>'
```shell
liuyi@scliu:13:36:40:$PS2='>>>'
liuyi@scliu:13:37:02:$echo $PS2
>>>
```
### 11.查看当前shell的所有变量
```shell
liuyi@scliu:13:37:20:$set
BASH=/bin/bash
BASHOPTS=checkwinsize:cmdhist:expand_aliases:extquote:force_fignore:histappend:hostcomplete:interactive_comments:login_shell:progcomp:promptvars:sourcepath
BASH_ALIASES=()
BASH_ARGC=()
BASH_ARGV=()
BASH_CMDS=()
BASH_LINENO=()
BASH_SOURCE=()
BASH_VERSINFO=([0]="4" [1]="2" [2]="46" [3]="2" [4]="release" [5]="x86_64-redhat-linux-gnu")
BASH_VERSION='4.2.46(2)-release'
COLUMNS=211
DIRSTACK=()
EUID=1005
GROUPS=()
HISTCONTROL=ignoredups
HISTFILE=/home/liuyi/.bash_history
HISTFILESIZE=1000
HISTSIZE=1000
HOME=/home/liuyi
HOSTNAME=scliu
HOSTTYPE=x86_64
ID=1005
IFS=$' \t\n'
LANG=zh_CN.UTF-8
LESSOPEN='||/usr/bin/lesspipe.sh %s'
LINES=52
LOGNAME=liuyi
LS_COLORS='rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=01;05;37;41:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.Z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.jpg=01;35:*.jpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.axv=01;35:*.anx=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=01;36:*.au=01;36:*.flac=01;36:*.mid=01;36:*.midi=01;36:*.mka=01;36:*.mp3=01;36:*.mpc=01;36:*.ogg=01;36:*.ra=01;36:*.wav=01;36:*.axa=01;36:*.oga=01;36:*.spx=01;36:*.xspf=01;36:'
MACHTYPE=x86_64-redhat-linux-gnu
MAIL=/var/spool/mail/liuyi
MAILCHECK=60
OPTERR=1
OPTIND=1
OSTYPE=linux-gnu
PATH=/usr/local/bin:/bin:/usr/bin:/usr/local/sbin:/usr/sbin:/home/liuyi/.local/bin:/home/liuyi/bin
PIPESTATUS=([0]="0")
PPID=2598
PROMPT_COMMAND='printf "\033]0;%s@%s:%s\007" "${USER}" "${HOSTNAME%%.*}" "${PWD/#$HOME/~}"'
PS1='\u@\h:\t:\$'
PS2='>>>'
PS4='+ '
PWD=/home/liuyi
SHELL=/bin/bash
SHELLOPTS=braceexpand:emacs:hashall:histexpand:history:interactive-comments:monitor
SHLVL=1
TERM=xterm
UID=1005
USER=liuyi
XDG_SESSION_ID=2
_='>>>'
big_city=changsha
colors=/home/liuyi/.dircolors

```
### 12.退出liuyi这个用户
```shell
liuyi@scliu:13:38:07:$exit
登出

```
### 13.新建一个用户zengqilin
```shell
[root@localhost ~]# useradd zengqilin

```
### 14.进入zengqilin的家目录
```shell
[root@localhost ~]# cd ~zengqilin
[root@localhost zengqilin]# 
```
### 15.返回当前用户的家目录
```shell
[root@localhost zengqilin]# cd
[root@localhost ~]#
```
