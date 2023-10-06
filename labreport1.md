**Lab Report 1**
```
  [user@sahara ~]$ cd
  [user@sahara ~]$
  [user@sahara ~]$ cd lecture1 
  [user@sahara ~/lecture1]$ 
  [user@sahara ~]$ cd lecture1
  [user@sahara ~/lecture1]$ cd messages
  [user@sahara ~/lecture1/messages]$ cd en-us.txt
  bash: cd: en-us.txt: Not a directory
```
  When running cd initially nothing happens because you dont say where to change the directory to. When you specify the destination with lecture1 it then goes to lecture1, however it cannot go to a file as an argument because it only accepts directories as arguments.
```
  [user@sahara ~]$ ls
  lecture1
  [user@sahara ~]$ ls lecture1
  Hello.class  Hello.java  messages  README
  [user@sahara ~]$ cd lecture1
  [user@sahara ~/lecture1]$ cd messages
  [user@sahara ~/lecture1/messages]$ ls es-ms.txt
  ls: cannot access 'es-ms.txt': No such file or directory
```
  When running ls initially it lists out what we have open accesss to which is simply the lecture1 directory which if we then type that after ls it displays a list of everything in that directory. Once again if you specify a file it doesn't show anything because there isn't a list of files/folders in a file.
```
  [user@sahara ~]$ cat

  [user@sahara ~]$ cat lecture1
  cat: lecture1: Is a directory
  [user@sahara ~]$ cd lecture1
  [user@sahara ~/lecture1]$ cd messages
  [user@sahara ~/lecture1/messages]$ cat ko.txt
  안녕 세계
```
  At first when you use cat it returns nothing because you are checking for what is inside of nothing. When you include lecture1 is shows what is it telling us that lecture1 is indeed a directory, and lastly if you are to direct yourself into the messages folder, if you cat a specific text file it returns whatever text is in that file.
