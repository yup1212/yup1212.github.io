# 终端常用命令
## 软连接
### windows 
mklink /J "[映射目录]" "[原目录]"

创建

    mklink [How to operate] "[映射目录]" "[原目录]"
删除

    rmdir "[映射目录]"
+ [How to operate] 
    + /D 构造目录的符号链接.默认是一个文件符号链接.
    + /H 构造一个硬链接，而不是符号链接.
    + /J 构造一个目录链接
+ [映射目录] 指定新链接的名字
+ [原目录] 目标目录的原文件路径

### ubuntu
ln -s [原目录] [映射目录]

创建

    ln [How to operate]  [原目录] [映射目录]
删除

    sudo rm -rf [映射目录]
+ [How to operate] 
    + f : 链结时先将与 dist 同档名的档案删除
    + -d : 允许系统管理者硬链结自己的目录
    + -i : 在删除与 dist 同档名的档案时先进行询问
    + -n : 在进行软连结时，将 dist 视为一般的档案
    + -s : 进行软链结(symbolic link)
    + -v : 在连结之前显示其档名
    + -b : 将在链结时会被覆写或删除的档案进行备份
    + -S SUFFIX : 将备份的档案都加上 SUFFIX 的字尾
    + -V METHOD : 指定备份的方式
    + --help : 显示辅助说明
    + --version : 显示版本