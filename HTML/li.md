#HTML标签的结束 
    
##1、列表
###1、有序列表   &nbsp;ol>li
 - `tpye`属性  &nbsp;设置序号的类型具体有1、，A、，Ⅰ、，㈠、等
 - `start`属性  &nbsp;表示序号的开头数字
###2、无序列表 &nbsp;ul>li
 - `type`属性 &nbsp;表示每列前面的标记点的类型
	- `disc`  &nbsp;实心圆点（默认）
	- `Circle`  &nbsp;空心圆点
	- `square`  &nbsp;方形点
###3、自定义列表  &nbsp;dl>dt>dd
    
##2、`video`标签 视频
 1. `src`属性 &nbsp;表示视频的来源
 2. `source`标签 &nbsp;表示不同视频格式的选择播放
 3. `type`属性&nbsp;表示视频的类型
 4. `comtrols`属性&nbsp;表示展示控件
 5. `autoplay`属性&nbsp;表示加载完了就马上播放
 6. `loop`属性&nbsp;表示循环播放
 7. `muted`属性&nbsp;规定视频的音频输出应该被静音。
 8. `preload`属性＆nbsp;用于与页面同时加载，并表示准备播放。但是`autoplay`掩盖该属性的。
 9. `poster`属性&nbsp;视频播放前的展示图片
 
    
 ```html
 <video width="300" height="300" controls="controls">
<source src="img/tunnel.mp4" type="video/mp4"></source>
<object width="" height="" type="application/x-shockwave-flash" data="myvideo.swf">
<param name="movie" value="myvideo.swf" />
<param name="flashvars" value="autostart=true&amp;file=myvideo.swf" />
</object>
当前浏览器不支持 video直接播放，点击这里下载视频： <a href="myvideo.webm">下载视频</a>
</video>
 ```
    
##3、`audio`标签 音频
 1. `src`属性 &nbsp;表示视频的来源
 2. `source`标签 &nbsp;表示不同视频格式的选择播放
 3. `type`属性&nbsp;表示视频的类型
 4. `comtrols`属性&nbsp;表示展示控件
 5. `autoplay`属性&nbsp;表示加载完了就马上播放
 6. `loop`属性&nbsp;表示循环播放


    
```html
<audio width="320" height="240" controls="controls">
  <source src="song.ogg" type="audio/ogg">
  <source src="song.mp3" type="audio/mpeg">
  <p>Your browser does not support the audio tag.</p>
</audio >
```
    