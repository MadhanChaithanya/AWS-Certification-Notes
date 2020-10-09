## Linux Series:

### Linux - The Operating System
* RedHat Linux, Ubuntu, Centos, SUSE etc are called as distributions.
* Distribution is Linux + software suite of applications, developer tools
* In this essence Linux is core of the operating system: _kernel_

#### Layers of Abstraction in Linux
* General Linux System Organization
![Preview](./Images/linux1.jpg)
* Layers are
    * Hardware
    * Kernel
    * User Process
* kernel is in charge for managing
    * Processes
    * Memory
    * Device Drivers
    * System Calls
        * fork
        * exec
* User Space:
    * Kernel allocates memory for user processes and this is called as userspace.
    ![Preview](./Images/linux2.jpg)
    * User: A user is an entity that can run processes and own files.

### Shell and Terminal:
* When we speak of the commandline we are referring to shell. Shell is a program takes commands and passes them to Operating System to carry out.
* Almost all the distributions a shell program called as bash is supplied.
* To interact with shell we need a terminal 

### Creating Linux Instances on the cloud
* Prerequisites
    * Softwares used in this series
        * Git Bash
        * Visual Studio Code
    * One free tier cloud account (AWS/Azure)
* Linux Distributions
    * Ubuntu 18
    * Centos 7
* Lets create a linux instance and login into that
![Preview](./Images/linux3.jpg)        

### Standard Input and Standard Output
* Linux processes use I/O streams to read and write data.
* Streams are very flexible, the source of input stream can be a file, device or it can be even the output stream of other process




### Linux Commands
* In the shell prompt we generally execute commands. Let's execute the some simple commands
```
date
cal
```
![Preview](./Images/linux4.jpg)
* Basic command syntax
```
<command> <args>
echo hello
```
* Arguments of two types
    * Positional arguments:
    ```
    <command> <arg1> <arg2> ...
    cp 1.txt 2.txt
    ```
    * Named arguments:
    ```
    <command> --<argname> <argumentvlaue>
    ping -c 4 google.com
    ```
* __ls__: this command is used to list the contents of the directory
 ```
ls
ls -a
 ```
![Preview](./Images/linux5.jpg)
![Preview](./Images/linux6.jpg)
* __touch__: this command creates an empty file
```
touch 2.txt
```
* __cp__: this command copies files 
```
cp file1 file2
```



