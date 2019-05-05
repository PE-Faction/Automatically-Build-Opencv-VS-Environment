# opencv-vs环境自动配置工具
<br>
&emsp;&emsp;最近一直在学习pyqt,以前做东西，画界面一直是用的C++，最近一接触python画界面，感觉python真的对于护发有很大的好处。因为平时项目中，主要还是做图像方面比较多一些，也多将Visual Studio和opencv搭配使用，opencv的安装和在VS上的使用，对于初学者可能不是很友好，需要配置环境变量，然后在VS上配置属性表，之后才能使用，步骤有些繁琐，也很烦人，正好最近一直想找个小项目练练手，所以就写了这一个小的工具。
1.下载opencv，解压到某个文件夹
2.利用工具进行环境配置
&emsp;&emsp;首先如图所示，选中启动程序，点右键以管理员身份运行（因为需要更改注册表，所以采用这个方法），即可进入界面
<br>
<div align=center><img src="images/1.PNG" /></div>
<br>
程序界面情况如下所示:
<br>
<div align=center><img src="images/2.PNG" /></div>
<br>
点击打开目录，选中opencv的安装目录(一般该目录下有bulid和sources两个文件夹)，如图所示
<br>
<div align=center><img src="images/3.PNG" /></div>
<br>
<br>
<div align=center><img src="images/4.PNG" /></div>
<br>
接着选择自己VS的版本
<br>
<div align=center><img src="images/11.PNG" /></div>
<br>
程序会根据opencv的安装目录解析opencv的目录结构，然后选择配置32位或者64位的属性表。
<br>
<div align=center><img src="images/12.PNG" /></div>
<br>
最后选择opencv的版本（一般采用默认版本即可，不用选择）
<br>
<div align=center><img src="images/13.PNG" /></div>
<br>

这些选定之后，就可以点击配置环境，可得
<br>
<div align=center><img src="images/6.PNG" /></div>
<br>
接着点击生成属性表，程序文件夹中就会产生debug和release版本的属性表.
<br>
<div align=center><img src="images/7.PNG" /></div>
<br>
在建立项目后，在VS的属性管理器中添加以上生成的属性表，即可使用opencv的相关库（如果运行提示找不到一些库，可以重启或者注销电脑，让环境变量加载进去）。
<br>
<div align=center><img src="images/15.PNG" /></div>
<div align=center><img src="images/14.PNG" /></div>
<br>

&emsp;&emsp;**这个项目基础功能能实现，但肯定存在着诸多bug，另外这个程序的图标我换了半天，也没搞好，路过的大神有做过的，麻烦指点我一下，pyinstaller我弄了很长时间，那个.ico文件硬是添加不进去，为了不让自己患上忧郁症，我决定冷静一下。菜鸟作品，不喜勿喷！**
