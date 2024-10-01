# ncmdump
music: change filetype from .ncm to .mp3.  将网易云下载的.mcn格式音乐转化成.mp3格式

---
## 使用

### 使用`-h` 或 `--help` 参数来打印帮助
~~~
ncmdump -h
~~~

### 使用 -v 或 --version 参数来打印版本信息
~~~
ncmdump -v
~~~


### 处理单个或多个文件
~~~
ncmdump 1.ncm 2.ncm...
~~~

### 使用 -d 参数来指定一个文件夹，对文件夹下的所有以 ncm 为扩展名的文件进行批量处理
~~~
ncmdump -d source_dir
~~~

### 使用 -r 配合 -d 参数来递归处理文件夹下的所有以 ncm 为扩展名的文件
~~~
ncmdump -d source_dir -r
~~~


### 使用 -o 参数来指定输出目录，将转换后的文件输出到指定目录，该参数支持与 -r 参数一起使用
~~~
# 处理单个或多个文件并输出到指定目录
ncmdump 1.ncm 2.ncm -o output_dir

# 处理文件夹下的所有以 ncm 为扩展名并输出到指定目录，不包含子文件夹
ncmdump -d source_dir -o output_dir

# 递归处理文件夹并输出到指定目录，并保留目录结构
ncmdump -d source_dir -o output_dir -r
~~~
