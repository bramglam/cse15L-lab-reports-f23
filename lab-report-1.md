##Lab Report 1 - Remote Access and FileSystem (Week 1)

###Command: cd
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
This output simply changes the working directory to ./lecture1/messages, which is shown to the left of the $ sign. The output is not an error.
Path to File:

```shell

[user@sahara ~]$ cd ./lecture1/messages/es-mx.txt
bash: cd: ./lecture1/messages/es-mx.txt: Not a directory

```
The pwd (present working directory) is /home. The output attempts to change the directory to ./lecture1/messages/es-mx.txt, but this results in an error. The error is due to the fact that es-mx.txt is not a directory, but a file. Thus it cannot execute the command on a file.


###Command: ls
No arguments:

```shell
[user@sahara ~]$ ls
**lecture1**
```
The pwd (present working directory) is /home. The command had no arguments, meaning nothing came after command when entered. This command simply lists all the files and sub-directories in a working directory. The output is not an error. 

Path to Directory:

```shell
[user@sahara ~]$ ls ./lecture1/messages
ar-bh.txt  es-mx.txt
en-us.txt  zh-cn.txt
```
The pwd (present working directory) is /home. The command had an argument to display the files within a given directory, which was entered as a path to the directory. The output is not an error.

Path to File:

```shell
[user@sahara ~]$ ls ./lecture1/messages/es-mx.txt
ar-bh.txt  es-mx.txt
en-us.txt  zh-cn.txt
bash: /es-mx.txt: No such file or directory
```
The pwd (present working directory) is /home. The command attempts to list out all the files within a file instead of a directory, resulting in an error. The argument given to ls is a path to a file.

###Command: cat
No arguments:

```shell
[user@sahara ~]$ cat


```
The pwd (present working directory) is /home. This command attempts to read the contents of a file out. However, there were no arguments after the cat command, resulting in no output. The output is not an error.

Path to Directory:

```shell
[user@sahara ~]$ cat lecture1/messages
cat: lecture1/messages: Is a directory
```
The pwd (present working directory) is /home. The command cat takes the argument of a path to a directory. However, the command cat doesn't work to print the contents of a directory, only a file. Thus it is an error.

Path to File:

```shell
[user@sahara ~]$ cat lecture1/messages/en-us.txt
Hello World!
```
The pwd (present working directory) is /home. The argument entered after cat is a path to a file, and it prints the contents of the file. The output is not an error.

