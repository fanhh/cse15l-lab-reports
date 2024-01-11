## Lab1 Report

### ```cd```
#### - Example 1 (no arugments): ```[user@sahara ~]$ cd``` --> nothing
##### - it will show nothing because cd will bring you back to the root dir
#### - Example 2: ```[user@sahara ~]$  cd lecture1``` -->  ```[user@sahara ~/lecture1]$```
##### - it will show that that dir changes to lecture1
#### - Example 3: ```[user@sahara ~]$  cd lecture1/messages/en-us.txt``` --> ```bash: cd: lecture1/messages/en-us.txt: Not a directory```
##### - it will show and bash since you can not cd to a file 

### ```ls```
#### - Example 1 (no arugments): ```[user@sahara ~/lecture1]$ ls``` --> ```en-us.txt  es-mx.txt  zh-cn.txt```
#### - Example 2: ```[user@sahara ~]$  ls lecture1``` -->  ```en-us.txt  es-mx.txt  zh-cn.txt```
#### - Example 3: ```[user@sahara ~]$  ls lecture1/Hello.java``` --> ```lecture1/Hello.java```


### ```cat```
#### - Example 1 (no arugments): ```[user@sahara ~]$ cat``` --> terminal freeze
#### - Example 2: ```[user@sahara ~]$  cat lecture1``` -->  ```cat: lecture1: Is a directory```
#### - Example 3: ```[user@sahara ~]$  cat lecture1/Hello.java``` --> ```import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }```


![Image](dragon.jpeg)
