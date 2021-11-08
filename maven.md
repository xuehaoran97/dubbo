1.前往官网下载maven

![image-20211108141056509](/Users/xuehaoran/Library/Application Support/typora-user-images/image-20211108141056509.png)

2.解压

3.配置环境变量

```shell
vi ~/.bash_profile 
#maven
export M="/Users/xuehaoran/IdeaProjects/software/apache-maven-3.8.3"
export PATH="$M/bin:$PATH"
source ~/.bash_profile
mvn -v
```



4.配置阿里云镜像

```shell
vim /Users/xuehaoran/IdeaProjects/software/apache-maven-3.8.3/conf/settings.xml

```

```xml
 <mirror>
        <id>nexus-aliyun</id>
        <mirrorOf>*</mirrorOf>
        <name>Nexus aliyun</name>
        <url>http://maven.aliyun.com/nexus/content/groups/public</url>
</mirror>
```

