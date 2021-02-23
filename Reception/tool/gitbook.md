# gitbook安装与使用
1. 首先在全局安装 gitbook 客户端工具：
```
    npm install gitbook-cli -g
```
2. 创建book.json并安装 创建一个空的文件夹，并在这个文件夹中创建一个book.json文件
```
    {
        "gitbook":"2.x.x"
    }
```
    表示安装gitbook的2.x.x版本，以后可以扩展此文件安装更多的gitbook插件
```
    gitbook install   //局部安装
```
 > **注意:**上面的命令要在book.json的文件路径下打开**cmd**运行

3. 创建README.md 和 SUMMARY.md
 ```
    gitbook init   //初始化
 ```
    在你的作品目录中创建两个必需的文件 README.md 和 SUMMARY.md，README.md 是作品的介绍，SUMMARY.md 是作品的目录结构，里面要包含一个章节标题和文件索引的列表：

 ```html
    # Summary
    This is the summary of my book.
    * [section 1](section1/README.md)
        * [example 1](section1/example1.md)
        * [example 2](section1/example2.md)
            - [example 3](section1/example3.md)
    * [section 2](section2/README.md)
           * [example 1](section2/example1.md)
 ```

4. 运行服务，在编辑内容后可以实时预览：
```
    gitbook serve
```

 > **备注：**gitbook serve 要在gitbook目录文件路径下打开cmd运行

 服务器启动后，浏览器打开**http://localhost:4000**查看

5. 撰写完后可以生成静态网站用来发布：
```
    gitbook build
```
6. 更多命令帮助
```
    gitbook help
```
7. 自由切换版本
```
    gitbook ls-remote           //罗列出所有的版本号
    gitbook fetch 2.1.0         //选择其中一个版本切换安装
```
8. 更多插件 [参考链接](http://www.tuicool.com/articles/zee2ui)
