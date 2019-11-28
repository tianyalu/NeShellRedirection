# NeShellRedirection Shell之重定向

## 一、概念
### 1.1 重定向
Linux中万物皆文件，可以是屏幕，也可以是文件；重定向即数据流向的改变。  
* 输入重定向：<  
* 输出重定向：>  (>> 表示追加)  

命令             | 说明
------------    | --
command > file  | 将输出重定向到file
command < file  | 将输入重定向到file
command >> file | 将输出以追加的方式重定向到file
n > file        | 将文件描述符为 n 的文件重定向到file
n >> file       | 将文件描述符为 n 的文件以追加的方式重定向到file
n >& m          | 将输出文件m 和 n 合并
n <& m          | 将输入文件m 和 n 合并
<< tag          | 将开始标记tag 和结束标记tag 之间的内容作为输入  

![image](https://github.com/tianyalu/NeShellRedirection/blob/master/show/redirection.png)  

### 1.2 文件描述符
* 标准输入standard input 0 (默认设备键盘)     stdin    对应/dev/stdin
* 标准输出standard output 1 (默认设备显示器)  stdout   对应/dev/stdout
* 错误输出：error output 2 (默认设备显示器)   stderr   对应/dev/stderr  

实操：  
![image](https://github.com/tianyalu/NeShellRedirection/blob/master/show/redirection_command.png) 

