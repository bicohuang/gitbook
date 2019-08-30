##Nodejs如何安装
1、首先下载安装包 

官网：[点我](http://nodejs.cn/)

2、双击安装完成后，检查是否安装成功

命令行输入
```
    node -v         //返回nodejs的版本

    npm -v          //返回npm包管理器的版本
```
**注意**  如果之前已经安装过nodejs的话，想卸载干净，最好全局搜索`.npmrc`并删除,这个文件是记录了之前的`cache`和`prefix`的记录。

***修改环境变量*** 因为通常nodejs默认都会安装在C盘(window用户)或`/usr/local`(类linux用户)下，都涉及到管理员权限。有时候使用会不方便，这个时候就需要修改nodejs的环境变量。

类linux用户的方法
```
    //首先修改nodejs默认配置
    npm config set cache "/Users/ouxiaobao/node_cache/"  //改变默认cache位置
    npm config set prefix "/Users/ouxiaobao/node_global/" //改变默认全局node_module位置
    
    export PATH=$PATH:/Users/ouxiaobao/node_global/
```
而windows用户请参考本链接
```
//首先修改nodejs默认配置
npm config set cache "C:\nodejs\node_cache\"  //改变默认cache位置
npm config set prefix "C:\nodejs\node_global" //改变默认全局node_module位置

//然后记得修改环境变量Path,把C:\nodejs\node_global/node_modules添加进去
```
[windows参考资料](http://blog.csdn.net/pengpegv5yaya/article/details/51885829)

##如果发现npm命令无法安装，或全局命令找不到

全局搜索.npmrc并删除,这个文件是记录了之前的`cache`和`prefix`的记录。就是它搞得鬼，通常是放在`C:\Users（用户）\你的用户名.npmrc`