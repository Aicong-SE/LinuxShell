[toc]

## 后台运行

**暂时放后台运行**

在命令的最后加上 & ,可以把这个命令放到后台执行, 关闭当前终端会终止

```shell
watch  -n 10 sh  test.sh  &  #每10s在后台执行一次test.sh脚本
```

**前台正在执行的命令移到后台**

```shell
ctrl + z  # 移动到后台 且 暂停
```

**查看当前有多少在后台运行的命令**

```shell
jobs  # 只能查看当前终端放到后台的命令
```

**将后台运行的命令移动到前台继续运行**

```shell
fg %jobnumber  # jobnumber 是命令编号
```

**启动后台暂停的命令**

```shell
bg %jobnumber  # jobnumber 是命令编号
```

**终止后台命令**

```shell
① jobs 查看 jobnumber, kill %jobnumber
② ps 查看进程号, kill pid
```

**后台运行命令**

```shell
nohup 命令 & 
```

