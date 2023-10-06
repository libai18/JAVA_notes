# 开始

韩老师说:
再牛的程序员都是从小白开始,既然开始了,就全心投入学好技术

# 小技巧

## eclipse代码缩写

```java
main+Alt+/=		public static void main(String[]args){}
sysout			就可以打出system.out.println();
```



#  Test.java 到 Test.class

<img src="java image/1.png" style="zoom:50%;" /> 

先使用javac命令编译.java文件生成.class文件，然后使用java命令在Java虚拟机上运行生成的.class文件。

下面是转换的步骤：

1. 确保已经安装了Java开发工具包（JDK），它包含了Java编译器（javac）。

2. 打开命令行终端（Windows上是命令提示符，Mac和Linux上是终端）。

3. 使用cd命令切换到包含.java文件的目录。例如，如果.java文件位于C:\myproject目录下，可以使用以下命令切换到该目录：

```
cd C:\myproject
```

4. 在命令行中输入以下命令编译.java文件：

```
javac Test.java
```

5. 执行以上编译命令后，如果没有错误，将会生成与.java文件同名的.class文件。

6. 使用Java虚拟机（JVM）运行生成的.class文件。在命令行中输入以下命令：

```
java Test
```

# JDK 基本介绍

1) JDK 的全称(Java Development Kit Java 开发工具包)

JDK = JRE + java 的开发工具 [java, javac,javadoc,javap 等]

## JRE 基本介绍

1) JRE(Java Runtime Environment Java 运行环境)

JRE = JVM + Java 的核心类库[类]

2) 包括 Java 虚拟机(JVM Java Virtual Machine)和 Java 程序所需的核心类库等，如果想要运行一个开发好的 Java 程序，

计算机中只需要安装 JRE 即可。

## JDK、JRE 和 JVM 的包含关系

1) **JDK = JRE +** **开发工具集**（例如 Javac,java 编译工具等)
2) **JRE = JVM + Java SE** **标准类库**（java 核心类库）
3) 如果只想运行开发好的 .class 文件 只需要 JRE

# 环境变量

- 看一个现象

"在dos命令行[快捷方式win+r]中敲入javac,出现错误提示。"

​       <img src="java image/2.png" style="zoom:50%;" /> 

​	原因分析
错误原因:当前执行的程序在当前目录下如果不存在,win10系统会在系统中已有的一个名为path的环境变量指定的目录中查找。如果仍未找到,会出现以上的错误提示。所以进入到jdk安装路径\bin目录下,执行javac,会看到javac参数提示信息。

- 配置环境变量

1.我的电脑--属性--高级系统设置--环境变量
2.增加JAVA_HOME环境变量,指向jdk的安装目录d:\program\hspjdk8 
3.编辑path环境变量,增加%JAVA HOME%\bin"
4.打开DOS命令行,任意目录下敲入javac/java。如果出现javac的参数信息,配置 成功。

```dos
java -version 查看版本
```



# Hello world



```java
//对代码的相关说明
//1. public class Hello 表示 Hello 是一个类,是一个 public 公有的类
//2. Hello{ } 表示一个类的开始和结束
//3. public static void main(String[] args) 表示一个主方法,即我们程序的入口
//4. main() {} 表示方法的开始和结束
//5. System.out.println("hello,world~"); 表示输出"hello,world~"到屏幕
//6. ;表示语句结束
public class Hello {
	//编写一个 main 方法
	public static void main(String[] args) {
		System.out.println("韩顺平教育 hello");
	}
}
```















