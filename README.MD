最近压力有点大，给自己找点事做做，抓包试试做个百度网盘的第三方API

代码很烂，作者很懒，目测是会有各种问题23333

用的是Python，也不准备老老实实的按照规范写代码，就这样吧233333

# 进度

### 已实现功能

+ 模拟登陆

+ 多线程下载单个文件

+ 每下载一个文件块检测一次网盘文件是否被修改，如果被修改就报错、删除临时文件并退出

### 下一步准备实现的功能

+ 获取对应文件夹下文件信息（已实现参数加密部分）

+ 断点续传

### 一些困难
 
因为玄学问题，断点续传做了一下午没有搞定，下载下来的文件内容混乱，周末要补考，要开始复(yu)习了23333最近基本不会更新代码

等补考结束准备重修的那段时间应该可以静下心来重新梳理一下思路并再次整理代码

# 命名的说明

### 1.recode和info

recode一般指不会经常变化的信息，如登录信息(其实就是cookies)

info一般指经常变化的信息，如下载进度等信息(暂时还未完成)

### 2. YunPan类

YunPan类是暴露给直接使用者的类，但是正常情况下并不会承担太多逻辑功能，以便于~~在没有文档的情况下查看API~~利用跳转理清代码思路