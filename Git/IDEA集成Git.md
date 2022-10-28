# 1. 配置Git忽略文件

>为什么要忽略？
>与项目的实际功能无关，不参与服务器上部署运行。把它们忽略掉能够屏蔽IDE工具之间的差异。

>怎么忽略？
>1）创建忽略规则文件 **xxxx.ignore**(前缀名随便起，建议是git.ignore)
>建议放在家目录下

git.ignore文件模板内容如下：
```
# Compiled class file 
*.class

# Log file 
*.ctxt

# Mobile Tools for Java(J2ME)
*.jar
*.war
*.nar

# virtual machine crash logs
*.classpath
*.project
*.settings

```

>2)在.gitconfig文件中引用忽略配置文件

```
[user]
	name = 
	email = 
[core]
	excludesfile = 
```