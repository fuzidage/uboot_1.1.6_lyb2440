##1.添加uboot1.1.6源码包

##2.添加补丁v0.1
使其能在2440开发板运行，参考2410实现，暂时还只是支持nor启动

##3.添加补丁v0.2
支持从nand启动,但是uboot还没有集成nand功能,所以nand命令暂时还不能使用,只是单独实现了从nand中重定位代码到sdram的功能

##4.添加补丁v0.3
支持uboot中的nand相关命令

##5.添加补丁v0.4
支持mtd命令和分区,支持jffs命令

##6.添加补丁v0.5
新增了支持dm9000网卡功能，能够使用ping和tftp下载。
原始的uboot1.1.6的dm9000.c无法进行tftp下载，ping也有的时候出问题。
参考高版本的uboot1.3.4 dm9000.c的实现拿过来移植.

