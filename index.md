## Lab1 Report

### ```cd```
#### - Example 1 (no arugments): ```[user@sahara ~]$ cd``` --> nothing
##### - it will show nothing because cd will bring you back to the root dir
#### - Example 2: ```[user@sahara ~]$  cd lecture1``` -->  ```[user@sahara ~/lecture1]$```
##### - it will show that that dir changes to lecture1 since we move to this working dir with cd
#### - Example 3: ```[user@sahara ~]$  cd lecture1/messages/en-us.txt``` --> ```bash: cd: lecture1/messages/en-us.txt: Not a directory```
##### - it will show and bash since you can not cd to a file because it's expecting a dir path not a file path

### ```ls```
#### - Example 1 (no arugments): ```[user@sahara ~/lecture1]$ ls``` --> ```en-us.txt  es-mx.txt  zh-cn.txt```
##### - It shows all the files and dir within the current working dir
#### - Example 2: ```[user@sahara ~]$  ls lecture1``` -->  ```Hello.class  Hello.java  messages  README```
##### - It shows that we go into this dir and show all the files and dir within this dir or files but we are not changing our current working dir
#### - Example 3: ```[user@sahara ~]$  ls lecture1/Hello.java``` --> ```lecture1/Hello.java```
##### - It shows the path I provided to the file because it confirms the existence of the file by listing the path provided.


### ```cat```
#### - Example 1 (no arugments): ```[user@sahara ~]$ cat``` --> nothing
##### - The reason it's outputting nothing because it's waiting for user to enter inputs
#### - Example 2: ```[user@sahara ~]$  cat lecture1``` -->  ```cat: lecture1: Is a directory```
##### - The reason it's outptting this because cat is used to read and concatenate files not dir
#### - Example 3: ```[user@sahara ~]$  cat lecture1/Hello.java``` --> 
```
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
##### - The reason it's ouptting this because it's reading the entire files and concatenated and output in the terminal


![Image](dragon.jpeg)
