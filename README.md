## 2020.7.23发现问题如下：
+ 该文件并没有双电池，只是用的是键盘的电池，没有用屏幕的
+ 但是当你拆掉屏幕后，电脑用的是屏幕的电池
+ 使用黑苹果会加快surface book电池的损耗，不建议使用
# SurfaceBook-Hackintosh
surfaceBook1 黑苹果


第一次搞黑苹果，经过我3天的摸索，终于让我的surfaceBook一代吃上个苹果了！
我的clover是基于下面这个大佬的，所以使用或者安装时有什么问题，都可以去这个帖子看看：
http://bbs.pcbeta.com/forum.php?mod=viewthread&tid=1806282&highlight=surface

但是上面这个帖子的clover是surface pro 4的，无法驱动surfaceBook的双电池，我参考了国外一个大佬的clover：

https://www.insanelymac.com/forum/topic/311874-guidedeprecated-installing-os-x-10114-10123-on-surface-book/


改出了一个适合surfaceBook一代使用双电池的macOS 10.14.6的clover！（先声明！使用后出什么问题，我不负责的哈！只是提供出来给大家学习，交流！）

不工作：
+ wifi
+ 蓝牙
+ 侧边音量按键
+ 摄像头
+ 键盘锁定大写按键灯不亮（可以切换大小写）
无线网卡的选择

无线网卡用的cf-812AC,贼稳定，注意：cf-811ac不稳定。如果你没有买到无线网卡就想使用黑苹果上网，可以用你的安卓手机通过usb共享网络先上网的！！！

os x安装下面的驱动就可以usb共享网络了
https://github.com/jwise/horndis


效果图：
![image](http://bbs.pcbeta.com/data/attachment/forum/201910/14/153756me2578ku7wu3lct7.png)


电源：

![image](http://bbs.pcbeta.com/data/attachment/forum/201910/14/153858d5zqo3ljczu4zjc3.png)

安装教程：
我是直接单系统的，如果你也是。就不需要去分区了，直接更换efi文件就好了（完全删除原本的clover后再复制进去，不要直接替换！！）

参考surface pro6 黑苹果的教程：
http://www.ishenping.com/ArtInfo/1292954.html

注意
无限重启？不要慌！！
详细的看下面这个帖子！！！

http://bbs.pcbeta.com/forum.php?mod=viewthread&tid=1806282&highlight=surface

ps：我是无限重启，然后给u盘使用10.13的clover去引导开机，然后赶紧重建缓存，就可以开机了，然后再也不需要u盘引导了！

没有Tools文件夹？
不要慌！自己去下载重建缓存的软件就好了

