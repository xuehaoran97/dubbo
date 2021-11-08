1.首先下载zookeeper 密码092014

```shell
sudo wget https://dlcdn.apache.org/zookeeper/zookeeper-3.5.9/apache-zookeeper-3.5.9-bin.tar.gz
```



2.解压zookeeper压缩文件到自定义文件夹

```shell
mkdir zookeeper
tar -vxf apache-zookeeper-3.5.9-bin.tar.gz -C zookeeper

```

3.复制conf文件夹下的zoo_sample.cfg文件

```shell
cp zoo_sample.cfg zoo.cfg
然后修改配置
```

4.配置环境变量

```shell
sudo vi ~/.bash_profile
#zookeeper
export ZK_HOME=/usr/local/zk/apache-zookeeper-3.6.2-bin/  --你zk的目录
export PATH=$PATH:$ZK_HOME/bin　
source ~/.bash_profile
```

5.启动zookeeper

```shell
zkServer.sh start
```

Note:

本机zookeeper的存储地址为

```shell
/Users/xuehaoran/IdeaProjects/software/zookeeper/apache-zookeeper-3.5.9-bin/b
```

zookeeper常用命令
```shell
执行sh zkServer.sh start即可

停止：sh zkServer.sh stop

查看状态：sh zkServer.sh status
```
