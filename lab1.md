# Lab Report 1 - Remote Access and FileSystem
**1. an example of using `cd`, `ls`, `cat` with no arguments.**
* cd
  ```
  [user@sahara ~]$ pwd
  /home
  [user@sahara ~]$ cd
  [user@sahara ~]$ pwd
  /home
  ```
* ls
  ```
  [user@sahara ~]$ ls
  lecture1
  ```
* cat
  ```
  [user@sahara ~]$ cat
  read md
  read me
  ```
**2. an exmaple of using `cd`, `ls`, `cat` with a path to a *directory* as an argument.**
* cd
  ```
  [user@sahara ~]$ pwd
  /home
  [user@sahara ~]$ cd lecture1/
  [user@sahara ~/lecture1]$ pwd
  /home/lecture1
  ```
* ls
  ```
  [user@sahara ~]$ ls lecture1/
  Hello.class  Hello.java  messages  README
  ```
* cat
  ```
  [user@sahara ~]$ cat lecture1/
  cat: lecture1/: Is a directory
  ```
**3.  an example of using `cd`, `ls`, `cat` with a path to a *file* as an argument.**

    
