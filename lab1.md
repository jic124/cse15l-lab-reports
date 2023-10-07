# Lab Report 1 - Remote Access and FileSystem

**`cd`** change directory \
**`ls`** list files \
**`cat`** view (or create) file
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
  As shown by the `~` sign and `pwd` command, the working directory is *home* for this and all other examples for question 1.
<br>
  
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

    
