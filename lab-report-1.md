##Lab Report 1 - Remote Access and FileSystem (Week 1)

Command: cd
No Arguments:
```shell

[user@sahara ~/lecture1]$ cd
[user@sahara ~]$ 

```
The working directory where the command was run is /home/lecture1 .

The output simply changed the directory to the root directory, removing ~/lecture1 from the square brackets. It had no arguments because nothing was included after the command. The output is not an error.


Path to Directory:
```shell

[user@sahara ~]$ cd ./lecture1/messages
[user@sahara ~/lecture1/messages]$ 

```
The working directory where the command was run is /home. 
Path to File:

```shell

[user@sahara ~]$ cd ./lecture1/messages/es-mx.txt
bash: cd: ./lecture1/messages/es-mx.txt: Not a directory

```
The pwd (present working directory) is /home.
Command: ls
No arguments:

```shell
[user@sahara ~]$ ls
**lecture1**
```
The pwd (present working directory) is /home.
Path to Directory:

```shell
[user@sahara ~]$ ls ./lecture1/messages
ar-bh.txt  es-mx.txt
en-us.txt  zh-cn.txt
```
The pwd (present working directory) is /home.
Path to File:

```shell
[user@sahara ~]$ ls ./lecture1/messages/es-mx.txt
ar-bh.txt  es-mx.txt
en-us.txt  zh-cn.txt
bash: /es-mx.txt: No such file or directory
```
The pwd (present working directory) is /home.
Command: cat
No arguments:

```shell
[user@sahara ~]$ cat


```
The pwd (present working directory) is /home.
Path to Directory:

```shell
[user@sahara ~]$ cat lecture1/messages
cat: lecture1/messages: Is a directory
```
The pwd (present working directory) is /home.
Path to File:

```shell
[user@sahara ~]$ cat lecture1/messages/en-us.txt
Hello World!
```
The pwd (present working directory) is /home.

