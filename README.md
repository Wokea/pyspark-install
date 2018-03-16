# pyspark-install
this repository  is used to memorize the process of installing pyspark 
------------------------------------------------------------------------------------------------------------------------------------------
#                                Windows本地安装pyspark
------------------------------------------------------------------------------------------------------------------------------------------
Author：Wokea
Date：2018/3/16
------------------------------------------------------------------------------------------------------------------------------------------

准备工作：
1.安装python与pycharm
2.修改环境变量(pip，python)

在python安装好了以后，正式进入pyspark的安装
3.去官网下载spark包，python版本2.7的安装1.6.0；python版本3.5的安装2.1.0
4.下载好spark以后解压，保存路径：D:\spark\spark-2.1.0-bin-hadoop2.7
5.去pycharm里面设置两个东西：
一为run 配置的环境变量，添加，SPARK_HOME=D:\spark\spark-2.1.0-bin-hadoop2.7；PYTHONPATH=D:\spark\spark-2.1.0-bin-hadoop2.7\python
二为设置project structure = 把D:\spark\spark-2.1.0-bin-hadoop2.7\python\lib\ 这个路径下的两个包添加到内容跟目录下，相当于导入包
6.下载好py4j，鬼知道这是什么东东，反正pyspark和python连接需要的
7.去python安装目录下找到lib\site-packages\，在这个路径下新建文件：pyspark.pth （将spark的python路径放进去，也就是D:\spark\spark-2.1.0-bin-hadoop2.7\python）
8.重启pycharm即可运行成功，大功告成
------------------------------------------------------------------------------------------------------------------------------------------
