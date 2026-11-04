# Python 学习笔记

## 常用指令

```
import xx 导入
from xx import xx
import xx as xx

pip install 包名
pip uninstall
pip freeze = pip list 列出
```

Python join() 方法用于将序列中的元素以指定的字符连接生成一个新的字符串。

## os模块常用用法

```
os.getcwd() 得到当前的工作目录
os.listdir() 返回制定目录下的所有文件和目录名
os.path.dirpath() 获取路径名称
os.path.abspath() 获取绝对路径
os.path.basename() 获取当前的文件名称
os.replace(old，new) 将文件重命名
os.listdir() 返回制定目录下的所有文件和目录名
os.path.dirpath() 获取路径名称
os.path.join(path,name) 将名称为name的字符串与path路径拼接
os.path.getsize(filename) 获取文件的大小
os.path.split() 返回一个文件的目录名和文件名
```

## sys模块常用用法

```
sys.platform 得到运行的操作系统环境
sys.path 是一个list,指明所有查找module，package的路径.
sys.getfilesystemencoding() 获取pyhton解释器默认编码
```

## time模块常用用法

```
time.sleep() 暂停的秒数
time.localtime([sec]) 时间元组
time.gmtime() 不按时区
time.time() 时间戳
time.asctime 时间转换为如下形式：'Sun Jun 20 23:21:05 1993'
time.strptime(string[,format]) 根据格式解析表示时间的字符串
time.mktime(t)将 struct_time类型的时间转换为时间戳类型。
	%a-->星期的缩写
	%A-->完整的星期的名称
	%b-->月份的缩写
	%B-->完整的月份名称
	%c-->'Wed Mar 20 21:40:19 2019'格式
	%d-->十进制数格式的日期[01,31]
	%H-->小时（24小时制） 十进制数[00,23]
	%I-->小时（12小时制） 十进制数[01,12]
	%j-->一年中的一天（十进制数）[001,366]
	%m-->月份（十进制数）[01,12]
	%M-->分钟数（十进制数）[00,59]
	%p-->AM或PM
	%S-->秒数[00,59]
	%U-->一年中的周数（星期日作为一周的第一天）十进制数[00,53],第一个星期日之前的所有日子被认为是第0周。
	%w-->星期数（十进制数）[0,6]
	%W-->一年中的周数（星期一作为一周的第一天）十进制数[00,53],第一个星期一之前的所有日子被认为是第0周。
	%x-->日期表示（月/日/不带世纪的年份）例如'03/20/19'
	%X-->时间表示（时:分:秒）例如'21:56:34'
	%y-->不带世纪的年份(十进制数)[00,99]
	%Y-->带世纪的年份(十进制数)
	%z-->时区偏移指示与格式+ HHMM或-HHMM形式的UTC / GMT的正或负时差，其中H表示十进制小时数字，M表示小数分钟数字[-23：59，+ 23：59]。
	%Z-->时区名称，例如'中国标准时间'
	%%-->'%'字符。
```

## datetime模块常用用法

```
datetime.datetime.now() 当前的时间
datetime.date.fromtimestamp() 把时间戳转化为datetime类型
datetime.timedelta(4)
datetime.timedelta(hours=4)
x.replace(year=299,month=11,day=30)
```

## random模块常用用法

```
random.randit(1,10) 返回1-10之间的一个数字
random.randrange(1,10,2) 取10中的偶数
random.choice(str) 取给定字符中的一个
random.sample(str,4) 在随机字符中取四个
random.random() 随机生成浮点数
random.shuffle(a) 打乱list
```

## hashlib模块常用用法

```
m = hashelib.md5(bytes) 指定变量对象 hashelib.sha256(bytes)
m.update(bytes) 进行加密 m.update(str.encode("utf-8"))
m.digest() 消化
m.hexdigest() 16进制消化
```

## shutil模块常用用法

```
shutil.copyfile(file1,file2) 复制文件内容
shutil.copy(,) 复制全部
shutil.copytree(,,ignore=shutil.ignore_patterns(忽略的文件名)) 复制文件夹
shutil.make_archive("压缩路径","压缩形式","文件路径") 压缩文件
shutil.unpack_archive("文件路径","压缩路径")
```

## re模块常用用法

```
re.search 从同开始匹配
re.findall 以列表形式返回
x.group 把匹配到的分组
```
