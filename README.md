Java 环境变量配置 
====

## 准备工具

Java Jdk下载地址： 
[JDK 32位](http://download.oracle.com/otn-pub/java/jdk/8u111-b14/jdk-8u111-windows-i586.exe)
[JDK 64位](http://download.oracle.com/otn-pub/java/jdk/8u111-b14/jdk-8u111-windows-x64.exe)
Eclipse
[Eclipse 32位](http://ftp.jaist.ac.jp/pub/eclipse/technology/epp/downloads/release/neon/1a/eclipse-java-neon-1a-win32.zip);
[Eclipse 64位](http://ftp.jaist.ac.jp/pub/eclipse/technology/epp/downloads/release/neon/1a/eclipse-java-neon-1a-win32-x86_64.zip);

## 安装JDK

打开下载的JDK文件  --- 下一步
![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/1.png)

下一步 -- 记住这个安装目录待会要去找这个目录

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/2.png)
![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/3.png)

接下来系统会自动安装JRE 我们下一步

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/4.png)
![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/5.png)
![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/6.png)
  安装完成

## 配置环境变量

共要配置三个环境变量 

- JAVA_HOME  这个要新建
- CLASSPATH  这个要新建
- Path       这个需要编辑 编辑 编辑

找到我的电脑-- 右键属性

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/10.png)

点击高级系统设置
![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/11.png)

切换到“高级”选项 --- 点击环境变量

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/12.png)

点击下面的 -- 新建

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/17.png)

找到我们JDK安装的目录 复制路径 我这里是 `C:\Program Files\Java\jdk1.8.0_101`

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/13.png)

变量名填写 `JAVA_HOME`
变量值是我们刚刚复制的 `C:\Program Files\Java\jdk1.8.0_101`

然后点击确定

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/14.png)

继续新建 `环境变量`

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/17.png)

变量名填写 `CLASSPATH`
变量值是我们刚刚复制的 `.;%JAVA_HOME%\lib` 注意前面有个点也要复制

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/15.png)

继续找到Path 变量
点击编辑 重要的事情说三遍
`编辑`
`编辑`
`编辑`

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/18.png)

在变量值后面追加 `;%JAVA_HOME%\bin`  
注意：一定不要修改前面的值 有分号隔开

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/16.png)

到这我们的环境变量就配置完毕

## 测试环境变量

开始运行 `cmd`   --- 直接回车

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/19.png)

输入 `javac`

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/20.png)

如果出现下面第一个图片, 就说明配置成功了
第二个则是有问题

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/21.png)
![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/22.png)


## 解压运行Eclipse

解压刚刚下载好的Eclipse 

解压 到当前文件夹

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/7.png)

这就是解压出来的文件夹 -- 打开它

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/8.png)

双击`eclipse` 运行`Eclipse`

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/9.png)

出现下面的 界面 Eclipse 安装完毕

![](http://edustack-10027546.cos.myqcloud.com/images/Jdk-config/23.png)

Java 配置完毕

## 分享
分享更多黑科技[admxj.com](http://admxj.com "Mail")

如果你有好的意见或建议，欢迎联系我们[mail](mailto:admin@admxj.com "Mail")

