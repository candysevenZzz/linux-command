# linux-command

  ##  [解释chmod 权限777 -rwxrwxrwx](https://blog.csdn.net/yihui8/article/details/6975786)
  
  ---

  含义 **r w x**     **Read Write eXecute**    **4    2    1** 
  ---
                                                          
  -rw-r--r--  1 bu users  2254 2006-05-20 13:47 tt.htm
  
  ----
  
    从第二个字符起rw-是说用户bu有读、写权，没有运行权，接着的r--表示用户组users只有读权限，没有运行权，最后的r--指其他人（others）只有读权限，
  没有写权和运行权。这是系统默认设置，我可以改写tt.htm，同组的人和其他人只有权读，没人有权运行，因为只是一个html文件，不必运行。
    
    ---
    如 777 该登录用户（可以用命令id查看）、他所在的组和其他人都有最高权限
    
    如果用命令chmod 777 tt.htm，结果：-rwxrwxrwx  1 bu users 2254 2006-05-20 13:47 tt.htm    任何人都有读、写、运行三项权限。
    ---
