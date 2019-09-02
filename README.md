# electron-ffi-demo
electron 通过ffi 调用 dll的函数

参考网上例子搭建环境，基本都没有成功，主要还是环境和版本版本兼容问题，踩的坑记录下：

采用虚拟机先安装win7+sp1+IE11+.NET Framework 4.6.2
1. node 10.16.3
2. python 2.7
3. vs 2017
4. 执行：npm install –global –production windows-build-tools
5. 安装node-gyp npm install -g node-gyp
6. 创建项目目录，cd到目录下
	* 	npm init
	* 	npm install electron@4.2.9
	* 	npm install electron-rebuild
7. 安装ffi插件npm install ffi —save
8. 执行：.\node_modules.bin\electron-rebuild .\node_modules\ffi\


注意事项：
生成的dll里的调用函数需要设为导出函数
