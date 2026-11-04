# Windows 批处理

## 访问网址

```
explorer http://www.baidu.com
```

## 打开文件夹或文件

```
start D:\文件夹1
```

## 打开文件

```
start D:\文件夹1\test.txt
```

## 删除文件

```
del test.txt
del .\TEST\*.o
```

## 复制文件

```
copy *.txt 文件夹1
copy file1.txt 文件夹1
copy file2.txt 文件夹2
copy C:\Users\user\Desktop\welcome.txt D:\
```

## 重命名

```
ren *.txt *.mp3
ren  *.gif *.jpg
ren aa.txt bb.c
```

## 创建文件夹

```
md 文件夹1
md 文件夹2
md 文件夹3
```

## 创建文件

当前目录创建a.txt文件

```
cd.>a.txt
```

## 提取文件名

提取当前目录下扩展名为mp3的文件名，输出到mp3文件名.txt

```
dir *.mp3 /b>mp3文件名.txt
```

提取当前目录下的“深度睡眠”文件夹下的所有mp3文件名到文件

```
dir .\深度睡眠\*.mp3 /b>mp3文件名.txt
```

提取当前目录下所有文件的文件名到a.txt

```
dir c:\*.* >a.txt
```

## 输出文件的绝对路径信息

输出当前目录下mp3文件

```
dir *.mp3/b/s>MP3文件信息.txt
```

## 执行另一个批处理文件

```
call c:\code\run.bat
```

## 300s 后自动关机

```
shutdown -s -t 300
```

## 取消自动关机

```
shutdown -a
```

## 立刻重启

```
shutdown -r -t 0
```

## 60s后休眠

```
shutdown -h -t 60
```

## 隐藏文件夹

```
attrib +s +h D:\Secret
```

## 取消隐藏文件夹

```
attrib -s -h D:\Secret
```

## attrib命令

```
attrib +/-r
attrib +/-a
attrib +/-s
attrib +/-h
+ 设置属性
- 清除属性
r 只读属性
a 存档属性
s 系统属性
h 隐藏属性
```
