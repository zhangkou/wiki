install svn:
	aptitude install subversion
svn co svn://svn.openwrt.org/openwrt/trunk/

svn co svn://svn.openwrt.org/openwrt/branches/backfire  下载官网的源码
./scripts/feeds update -a     更新软件包
./scripts/feeds install -a    安装软件包
make menuconfig 进入定制界面（里面可以选择芯片的型号，集成的组件等等，根据实际情况选择）
defconfig
make V=99   （开始编译）
