# rEFind-minimal主题

[rEFInd](https://sourceforge.net/projects/refind/) 是一个非常好用的UEFI多系统引导器，支持图形界面，相当美观，但是rEFind的默认界面，相当难看，所以要进行主题美化，minimal是一个简介好看的主题  
## 用法  
### Windows  
首先安装[rEFind](https://sourceforge.net/projects/refind/))，下载下来之后解压，安装软件[Diskgenuis](https://www.diskgenius.cn/download.php)，打开，选择自己的硬盘，右侧双击EFI_ESP分区，将解压后的文件中有一个refind目录，将refind目录拖到EFI_ESP分区中的EFI目录下，在refind目录下创建themes目录，将本文件放到themes目录下，确保文件名为```rEFind-minimal```，然后在refind目录下将refind.conf复制到桌面，在最后一行添加
```
include themes/rEFInd-minimal/theme.conf
```
在放到refind目录下，覆盖原来的文件，然后重启就行了  
### linux(ubuntu)  
与windows一样，但是下载的时候在终端运行  
```
sudo apt install refind
```
然后在```/boot/efi/EFI```中，找到refind目录，进入到refind目录下，终端运行  
```
sudo echo "include themes/rEFInd-minimal/theme.conf" >> refind.conf
sudo refind-install
```
然后重启就行了
