# Lab Report 1 - Remote Access and FileSystem

**`cd`** change directory \
**`ls`** list files \
**`cat`** view (or create) file \
<br>
> ***files and directories used in this lab report***

![image](lecture1_display.png)

<br>

***


**1. an example of using `cd`, `ls`, `cat` with no arguments.**
* cd
  ```
  [user@sahara ~]$ pwd
  /home
  [user@sahara ~]$ cd
  [user@sahara ~]$ pwd
  /home
  ``` 
  As shown by the `~` sign and `pwd` command, the working directory is `/home` for this and all other examples for question 1. The command `cd` changes the working directory to an argument, however, there is no change in this situation because there are no arguments(/directories) provided to access. Hence, as illustrated by the execution of the second `pwd` command, the present working directory is still `/home` after running the code. 

<br>
  
* ls
  ```
  [user@sahara ~]$ ls
  lecture1
  ```
  The command `ls` displays all the directories and files present in the working directory. As the present working directory is `/home`, terminal returns the directories (and files) in the `/home` directory, which is `lecture1`, which you can also confirm from the image above.

<br>
  
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
* cd
  ```
  [user@sahara ~]$ cd lecture1/
  [user@sahara ~/lecture1]$ cd Hello.java
  bash: cd: Hello.java: Not a directory
  ```
* ls
  ```
  [user@sahara ~/lecture1]$ ls Hello.java
  Hello.java
  ```
* cat
  ```
  [user@sahara ~/lecture1]$ cat Hello.java
  import java.io.IOException;
  import java.nio.charset.StandardCharsets;
  import java.nio.file.Files;
  import java.nio.file.Path;

  public class Hello {
    public static void main(String[] args) throws IOException {
      String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
      System.out.println(content);
    }
  }
  ```

    
