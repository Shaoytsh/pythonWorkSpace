python下载第三方库或更新巨慢的解决方法
主要是更新源为国内镜像
方法/步骤
linux下，修改 ~/.pip/pip.conf (没有就创建一个)， 修改 index-url至tuna，内容如下：
 [global] index-url = https://pypi.tuna.tsinghua.edu.cn/simple

windows下，直接在user目录中创建一个pip目录，如：C:\Users\xx\pip，新建文件pip.ini，内容如下

 [global] index-url = https://pypi.tuna.tsinghua.edu.cn/simple
使用pip install 命令      pip install numpy       安装第三方库
提示pip版本过低时按照提示升级pip版本，重复以上操作，即可操作