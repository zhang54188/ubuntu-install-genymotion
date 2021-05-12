# ubuntu-install-genymotion



sudo apt-get install virtualbox
./genymotion-3.1.2-linux_x64.bin 
	如果报错 记得更改这个文件权限 chmod 777 genymotion-3.1.2-linux_x64.bin
就可以点击了 这两句话最好在一个位置执行 不然打开genymotion的时候会报错
接下来就是设置自己的模拟器了 账号在这个网址注册https://www.genymotion.com/account/create/
usage type选择gaming company type选择china
最后就是邮箱激活 
然后就能在ubuntu'中打开软件了 然后去设置你自己的模拟手机
注意：在直接拖入apk安装app时候会报错 An error occured while deploying the file. 
		This probably means that the app contains ARM native code
需要在打开你的模拟机型的时候拖入Genymotion-ARM-Translation_3.zip 
原因：是Genymotion模拟器使用的是x86架构，
          在第三方市场上的应用有部分不采用x86这么一种架构，所以在编译的时候不通过，报“APP not installed”，
          可以下载Genymotion提供的ARM转换工具包，将应用市场中的ARM架构的apk转换成Genymotion可以编译的x86架构；



卸载：
	genymotion卸载：首先找到你放这个genymotion-3.1.2-linux_x64.bin 下面运行./genymotion-2.7.2-linux_x64.bin --uninstall
	virtualbox卸载：dpkg -l |grep virtualbox 查询你安装的版本 dpkg -L virtualbox 这个是查询安装位置 
			运行：sudo apt-get remove virtualbox卸载


