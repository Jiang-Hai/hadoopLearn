linux java环境安装
===

* 从官网下载jdk压缩包
* 解压到合适的目录，这里是/usr/local
* 设置环境变量
   在/etc/profile 文件里添加如下几行：
    
  export JAVA_HOME=/usr/local/jdk1.8.0_131

 export JRE_HOME=$JAVA_HOME/jre

 export CLASSPATH=$JAVA_HOME/lib:$JRE_HOME/lib:$CLASSPATH

 export PATH=$JAVA_HOME/bin:$JRE_HOME/bin:$PATH

 #####也可以在某个具体用户的.profile文件里添加以上几行，用于指定该用户的java环境变量