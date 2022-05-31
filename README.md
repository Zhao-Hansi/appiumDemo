# appiumDemo
FYI 

##一、环境搭建

###1 java sdk的安装以及环境变量的配置
   官方网站 https://www.oracle.com/index.html下载java jdk1.8 ，下载完成后安装到本地。
bin目录下存放JDK用于开发的一些终端命令工具。常见的工具如：
''
   “javac”的作用是将java源文件编译为class文件(即自解码文件)；
“java”命令的作用是运行class文件。

db目录下是java开发的一个开源的关系型数据库；

include目录下是一些C语言的头文件；

jre目录下JDK所依赖的java运行时；

lib目录下存放JDK开发工具所依赖的一些库文件；

man目录下存放JDK开发工具的说明文档。

terminal中输入.bash_profile,如果你是第一次配置环境变量，可以使用“touch .bash_profile” 创建一个.bash_profile的隐藏配置文件.如果你是为编辑已存在的配置文件，则使用"open -e .bash_profile”命令;打开文件后输入
JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_161.jdk/Contents/Home
PATH=$JAVA_HOME/bin:$PATH:.
CLASSPATH=$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar:.
export JAVA_HOME
export PATH
export CLASSPATH
完成java home环境变量的配置，在终端输入java -version,看见下图则证明配置成功。


###2 Android sdk的安装以及环境变量的设置
在MAC上安装android-sdk，标准的安装方法是使用homebrew，运行如下命令：
brew update
brew install android-sdk
安装完成后配置.bash_profile，如果是zsh则配置.zshrc，在文件结尾加上export ANDROID_HOME="/usr/local/opt/android-sdk”
退出后执行
source~/.zshrc
使文件生效。

###3 appium desktop的安装
在GitHub的相关网站执行https://github.com/appium/appium-desktop/releases/tag/v1.21.0，选择相应的版本进行下载。

###4 adb命令的使用及连接手机的设备管理
终端输入adb，看到下图的输出则安装完成，配置环境变量。

