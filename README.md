## Linux Maven
### 安装
#### 下载
- [Maven下载](http://maven.apache.org/download.cgi)

#### 配置JDK
- 检查JDK和JAVA_HOME
```echo $JAVA_HOME,java -version```。
  - 若没有正确显示出JDK安装地址和JDK版本，进行配置。
  - 若正确显示，进行Maven相关设置。
- 配置 JAVA_HOME 和 JAVA_HOME
 - 安装JDK
 - 配置JAVA_HOME
``` export JAVA_HOME=/usr/lib/jvm/java-8-oracle```。
 - 再次运行echo `$JAVA_HOME`检查。

#### 配置Maven
- 解压 `tar -xvzf apache-maven-zip-name`
- 为Maven文件夹创建符号链接 `ln -s apache-file-name apache-maven`。
- 设置M2_HOME环境变量指向 apache-maven `export M2_HOME=/home/wangximing/software-install/apache-maven`。
- 添加apache-maven/bin 到PATH环境变量 `export PATH=$PATH:$M2_HOME/bin`
- 将上面两条命令添加到系统登录的shell脚本中
 - Ubuntu 中把上述两条命令添加到 ～/.bashrc
- 检查Maven `echo $M2_HOME`,`mvn -v`
