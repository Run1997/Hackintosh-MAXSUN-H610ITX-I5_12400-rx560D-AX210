# Hackintosh-MAXSUN-H610ITX-I5_12400-rx560D-AX210
铭瑄H610itx+i5-12400+RX560D+AX210，EFI+蓝牙驱动+WiFi驱动+USB驱动+安装工具

【主机配置清单】
芯片：英特尔 i5-12400 散片 									    
主板：铭瑄 H610iTX 挑战者2.5g												     
显卡：盈通 RX560D 4G								 
网卡：英特尔 AX210+8DB天线 
内存：海盗船 DDR4 3200 16G*2 		 				   				 
存储：三星 MZVL21T0HCLR-00B00 1T		   								 	  
散热：利民		 			  						 	 		 
电源：海韵 SSP-300SUG 300W    								 	
机箱：六鸽K2S V3									 

【需求】

1、MacOS系统13.4.1，单系统。

2、CPU睿频正常，不超频。

3、有线网络+声卡+USB接口+显卡需要能够正常使用。

4、WiFi+蓝牙+睡眠需要能够正常使用。

5、隔空投送+随航因为网卡原因，不做要求。

6、可以登陆和使用iCloud，AppStore等一系列苹果提供的服务。


【安装教程】
Ventura 13.4.1 镜像下载：https://yuexiang.fun/1556.html 进去里面找对应版本下载
安装教程请参考：https://yuexiang.fun/39.html 
注意事项：
1、我用的主板是铭瑄H610iTX，为了统一，首先扣掉主板电池恢复默认BIOS。
2、我用显卡是盈通RX560D 4G，并且使用了PCIE3.0显卡延长线，所以要进入BIOS把PCIE速率改为Gen3
3、铭瑄H610ITX如何设置U盘启动？开机后一直按F11会弹出选择框
4、安装上面的教程安装完后，成功进入Mac系统后，如何加载驱动：

将安装工具通过U盘拉到Mac系统下：安装OpenCore Configurator0.9.5、OCAuxiliaryTools

使用OpenCore Configurator0.9.3工具，在右上角菜单栏点击挂载系统的EFI文件夹

由于EFI中的OC是0.9.3，这里先升级为0.9.5 ，升级教程参考：https://zhuanlan.zhihu.com/p/564730631

升级完OC后，加载驱动：进入EFI文件夹，选择OC文件夹，找到config.plist 右键选择OCAuxiliaryTools打开

左边菜单栏选择Kernel, 然后在右边右键增加条目，把USB+蓝牙+WI FI驱动导入进去，然后保存，重启检查 驱动是否成功。

AX210 蓝牙驱动参考：https://bbs.pcbeta.com/viewthread-1939308-1-1.html （有问题可以爬楼看评论）

安装好系统后，切记不要登陆icloud 和 APPLE ID 等，否则可能黑号，需要先修改三码再进行登陆：https://www.bilibili.com/video/BV1454y167ML/
  
