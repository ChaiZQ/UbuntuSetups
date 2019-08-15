#Install cmake and git
```
sudo apt-get install cmake git
```
#use "cmake --version" to check your cmake version

#Cmake install(optional):
	第一步:下载源码
	1.1、下载Cmake-3.12.2源码包，官网下载地址:https://cmake.org/download/

	第二步：安装Cmake-3.12.2
	2.1、解压刚刚下载的cmake-3.12.2.tar.gz
	2.2、进入到cmake-3.12.2目录，执行命令:
	```
	sudo ./bootstrap
	```
	开始编译源码，大概一分钟编译完，耐心等待。
	编译完完成之后，执行命令:
	```
	sudo make
	```
	编译完成之后，执行命令:
	```
	sudo make install
	```
	开始安装Cmake-3.12.2到本机。

	2.3、到此，Cmake3.12.2就算是安装完成，现在执行命令:
	```
	cmake --version
	```
	返回版本号。

	第三步：配置带界面的Cmake（Cmake-gui）

	3.1、执行命令来安装Cmake-gui：
	```
	sudo apt-get install cmake-qt-gui
	```
	接着执行命令：
	```
	cmake-gui
	```
	查看是否安装成功。
