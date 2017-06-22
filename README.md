# someTips
### 聊天室
https://gitter.im/ vue-github
## this is an linked about some affairs
## 光标的相关事件:
https://developer.mozilla.org/en-US/docs/Web/API/Selection/removeRange
## 默认阻止换行事件发生: 
     $(this).bind('keydown',function(event){  
                    var e = event || window.event;  
                    if(!e.ctrlKey && e.keyCode ==13){  
                      return false;//这句话阻止原有的回车换行事件的冒泡执行  
                    }  
                }); 
                
### 判断用户是手机端还是pc端接入网站 
https://zhidao.baidu.com/question/266300125371439005.html?qbl=relate_question_0&word=%C8%E7%BA%CE%B5%C3%D6%AA%D3%C3%BB%A7%CA%C7%CA%D6%BB%FA%B6%CB%BB%B9%CA%C7pc%B6%CB%B7%C3%CE%CA%CD%F8%D5%BE
### //linux命令压缩和解压缩文件
### 解压：
tar –xvf file.tar 解压 tar包
tar -zxvf file.tar.gz 解压tar.gz
tar -xjvf file.tar.bz2 解压 tar.bz2
tar –xZvf file.tar.Z 解压tar.Z
tar -xvfj archive.tar.bz2 解压一个bzip2格式的压缩包
### 压缩：
tar -zcvf 压缩文件名.tar.gz 被压缩文件名 可先切换到当前目录下。压缩文件名和被压缩文件名都可加入路径。
tar -cvfz archive.tar.gz dir1 创建一个gzip格式的压缩包
### windows系统中端口被占用的解决方法：
netstat -ano  (查看占用进程)
tasklist|findstr "pid"  (查看占用程序)
taskkill /f /t /im node.exe  （杀掉占用进程程序）

### linux中端口被占用的解决方法:
lsof -i:8080
kill -9 pid
