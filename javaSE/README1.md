1.先下载 <font color="red">JDK</font>

> JDK(J2SE Development Kit), 也叫java开发包,运行Java必备环境

> 下载地址:java.sun.com(官网地址,根据实际需求下载相应版本,学习建议下载1.8版本,太新的相对不稳定)


2.安装 <font color="RED">JDK</font>

> 双击下载下来的exe(建议安装在 <font color="RED">C:\Program Files (x86)\Java\jdk1.8.0_91</font>下面)

> JDK安装完成后,在自定义安装中建议安装 JRE(J2SE Runtime Environment) java运行时环境 (java程序运行所需要的环境)

> 路径一般为: <font color="RED">C:\Program Files (x86)\Java\jre1.8.0_91</font>

> 注: JDK 本身带了个 JRE,提供给开发者测试用.单独安装个 JRE 可以给客户用


☆☆☆☆☆ 重点

3.配置<font color="RED">环境变量</font> (在系统变量做修改,所有用户都能用)

>* <font color="RED">Path</font> 最后面加上  <font color="RED">;C:\Program Files (x86)\Java\jdk1.8.0_91\bin</font> (<font color="RED">;</font>与前面的路径相隔)

>    也可新建变量 <font color="RED">JAVA_HOME</font>, 变量值  <font color="RED">C:\Program Files (x86)\Java\jdk1.8.0_91</font>

>	在 Path 的值最后加上  <font color="RED">;%JAVA_HOME%\bin</font>  (可在命令行里输入 echo %JAVA_HOME% 查看配置的环境变量)

>* <font color="RED">CLASSPATH</font>  <font color="RED">.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar</font>

>	      或者  <font color="RED">.;C:\Program Files (x86)\Java\jdk1.8.0_91\lib\dt.jar;C:\Program Files (x86)\Java\jdk1.8.0_91\lib\tools.jar</font>

>	(一定要加 . → 可找到当前路径下的class)


4.检验配置是否正确

> win+R 输入 cmd, 将路径定位到当前路径下

> 执行 <font color="RED">javac</font> HelloWorld.java (javac 编译命令)

> 当前路径下再输入 dir 会发现当前路径下多了个 HelloWorld.class 文件 (编译生成的文件)

> 再执行 <font color="RED">java</font> HelloWorld 执行该编译文件 (java 执行命令)

> 看是否打印出 HelloWorld (打印出来即配置完成)
