# AX88179-Usb3.0-Ubuntu18.04
Ax88179 USB3.0 Ubuntu 18.04 USB网卡驱动

官方源码下载地址

https://www.asix.com.tw/en/product/USBEthernet/Super-Speed_USB_Ethernet

下载文件解压

打开终端  cd  到解压目录

执行 make

注意：make install 会报错

使用 sudo make instlall 

再执行 modinfo ./ax88179_178a.ko | grep depend 

显示 depends:        usbnet,mii

执行 sudo insmod ax88179_178a.ko
