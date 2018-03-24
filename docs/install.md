# 环境安装

## [Mac]使用brew安装jdk1.8

安装java8

```
brew tap caskroom/versions
brew cask install java8
```

查看JAVA_HOME所在目录

```
$ /usr/libexec/java_home
/Library/Java/JavaVirtualMachines/jdk1.8.0_162.jdk/Contents/Home
```

配置环境变量

```
# Java语言设置
JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_162.jdk/Contents/Home
PATH=$JAVA_HOME/bin:$PATH
CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
```

查看是否安装成功

```
$ which java
/Library/Java/JavaVirtualMachines/jdk1.8.0_162.jdk/Contents/Home/bin/java
muming:bin muming$ java -version
java version "1.8.0_162"
Java(TM) SE Runtime Environment (build 1.8.0_162-b12)
Java HotSpot(TM) 64-Bit Server VM (build 25.162-b12, mixed mode)
```


