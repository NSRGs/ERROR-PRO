Python2编码问题
===============

### 暴力解决Python2编码问题

* python2
新建文件：`\Python27\Lib\site-packages\sitecustomize.py`

添加内容：
```
import sys
reload(sys)
sys.setdefaultencoding('utf8')
```

* pypy

新建文件：`\pypy2-v5.3.1-win32\site-packages\sitecustomize.py`

添加内容：
```
import sys
reload(sys)
sys.setdefaultencoding('utf8')
```
### 使用format格式化编码问题

* 当使用format格式化字符串的时候，如果几个参数的编码不一致将会出现编码问题, 如下: 
```
str_1 = '\xb9\xfe\xe0\xb6\xcd\xe6\xb6\xf9\xb5\xc4'
str_2 = '\xe5\x93\x88\xe5\x96\xbd\xe7\x8e\xa9\xe5\x84\xbf\xe7\x9a\x84'
str_3 = "gbk: {0}, utf8:{1}".format(str_1,str_2)
import chardet
print chardet.detect(str_3)
```
输出: {'confidence': 0.295945945945946, 'encoding': 'windows-1252'}

显然编码已经乱啦...

