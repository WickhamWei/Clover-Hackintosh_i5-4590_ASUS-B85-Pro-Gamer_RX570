# i5-4590-ASUS-B85-Pro-Gamer-RX570-Hackintosh
@[TOC](目录)
更新于2019-03-24
# 硬件需求
i5 4590
ASUS B85 Pro Gamer
AMD系列免驱动卡（笔者是蓝宝石RX574超白金）

# 什么东西工作
1.	CPU变频，H264编码及解码等。
2.	声卡网卡显卡。
3.	睡眠及唤醒。
4.	所有后置USB端口，前置3.0接口。（前置2.0请看**安装后操作**）
5.	后置音频输入及输出，前置音频输入及输出。
6.	独立显卡DP输出。

# 什么东西没测试
1.	主板自带的显示输出。（**没有独立显卡的同学请注意**⚠️，华硕技嘉等主流主板应该工作正常）
2.	主板自带的光数码输出。（手头没测试设备，但驱动显示工作正常）
3.	显卡的其他输出，例如HDMI和DVI。（只要不是阉割版的显卡应该都没问题）
# 什么东西不工作
1. ~~HEVC。~~（HD4600，RX570本身就不支持HEVC）
2.	~~DP和HDMI输出的音量调节。~~（苹果操作系统硬伤，安装软件可以解决）
# 安装前须知
1.	启用主板的核心显卡开关。（不是自动）
# 安装后操作
1.	安装Clover Configurator，挂载EFI盘，打开config配置文件。
2.	点击Rt Variables中点击Generate。
3.	点击System Parameters中CustomUUID下的Generate New。
4.	点击SMBIOS 将第三条内容拷贝到SmUUID 按<kbd>Win/Command</kbd> + <kbd>S</kbd>保存。
5.	去安装Sound Control 并重启以启用DP和HDMI输出的音量调节。重启完可以卸载，不受14天时间限制。
6.	如果出现AppStore无法登陆，删掉网络中全部内容。新建以太网（DHCP，可以上网）和以太网2（拨号，无需可以上网）并重启。
7.	要使用前置面板的2.0驱动请删除EFI-CLOVER-kexts-other-USBPorts.kexts，在链接: [USB-Inject-All官网](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/)下载最新的kexts放入，运行Kext Utility等待程序走完后重启即可。
8.	自己自定义USB驱动可以参考[黑果小兵](https://blog.daliansky.net/Intel-FB-Patcher-tutorial-and-insertion-pose.html)的教程，感谢他的付出！
# 其他EFI细节
1.	Clover版本4895
2.	本人自建USB.kext
# 下载地址
链接: [Releases](https://github.com/WickhamWei/i5-4590-ASUS-B85-Pro-Gamer-RX570-Hackintosh/releases)
失效请发邮件到wickhamwei@qq.com
![关于本机](https://img-blog.csdnimg.cn/20190320221606120.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzg0NTAzOQ==,size_16,color_FFFFFF,t_70)
关于本机
![驱动列表](https://img-blog.csdnimg.cn/20190320221637103.png)
驱动列表
![编码信息](https://img-blog.csdnimg.cn/20190324204655107.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzg0NTAzOQ==,size_16,color_FFFFFF,t_70)
编码信息
![前置输出 后置输出 光数码输出 显卡音频输出](https://img-blog.csdnimg.cn/20190324210120899.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzg0NTAzOQ==,size_16,color_FFFFFF,t_70)
前置输出 后置输出 光数码输出 显卡音频输出![前置输入及后置输入](https://img-blog.csdnimg.cn/20190324210140321.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzg0NTAzOQ==,size_16,color_FFFFFF,t_70)
前置输入及后置输入
