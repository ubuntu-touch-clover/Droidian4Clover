# 非官方的Droidian For 小米平板4


## 简单教程

* 在[releases](https://github.com/ubuntu-touch-clover/Droidian-Clover/releases)中下载需要的包。

* 进入twrp recovery

* 清除boot system vendor userdata分区并确保后三个分区的格式为ext4。

* 刷入提供的lineage 16底包。

* 刷入droidian-rootfs包。

* 刷入halium-boot.img到boot分区。

* （可选）刷入调试工具(devtools)。

* （可选）扩充文件系统到49G。
     将平板连接到电脑，打开cmd或者terminal在有adb的地方输入以下语句(不包含$ 那个只是为了好看~~)
     
   * 当然也可以把49g换成你平板的data分区大小，这里是64g版的data分区大小。
     
     ```shell
     $ adb shell
     $ e2fsck -fy /data/rootfs.img
     $ resize2fs /data/rootfs.img 49G
     ```
   
* 重启，enjoy~~

## 详细教程

[我的csdn博客](https://blog.csdn.net/github_38345754/article/details/120911574)

## 赞助
   如果你觉得这个项目帮到你了，可以考虑捐助我，让我做的更好！

![oh yeah](img.png)

