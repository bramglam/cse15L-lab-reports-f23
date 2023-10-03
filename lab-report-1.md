##Lab Report 1 - Remote Access and FileSystem (Week 1)##

Command: cd
No Arguments:
```shell

[user@sahara ~/lecture1]$ cd
[user@sahara ~]$ 

```

Path to Directory:
```shell

[user@sahara ~]$ cd ./lecture1/messages
[user@sahara ~/lecture1/messages]$ 

```
Path to File:

```shell

[user@sahara ~]$ cd ./lecture1/messages/es-mx.txt
bash: cd: ./lecture1/messages/es-mx.txt: Not a directory

```
Command: ls
No arguments:

```shell
[user@sahara ~]$ ls
**lecture1**
```
Path to Directory:

```shell
[user@sahara ~]$ ls ./lecture1/messages
ar-bh.txt  es-mx.txt
en-us.txt  zh-cn.txt
```
Path to File:

```shell
[user@sahara ~]$ ls ./lecture1/messages/es-mx.txt
ar-bh.txt  es-mx.txt
en-us.txt  zh-cn.txt
bash: /es-mx.txt: No such file or directory
```
Command: cat
No arguments:

```shell
[user@sahara ~]$ cat


```
Path to Directory:

```shell
[user@sahara ~]$ cat lecture1/messages
cat: lecture1/messages: Is a directory
```

Path to File:

```shell
[user@sahara ~]$ cat lecture1/messages/en-us.txt
Hello World!
```

