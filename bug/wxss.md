1、在组件中使用keyframes  
不生效的问题
问题代码如下：
```
@-webkit-keyframes __spinner-loading {
 from,
 to,
 40% {
  background-color: #888;
 }
 33.333% {
  background-color: red;
 }
}
```
原因： 33.333% 改为33%即可

2、button有一个最小尺寸，宽高无法设置的小于这个尺寸。  

3、wxss不支持部分css3选择器。

4、小程序view中英文数字不换行的问题，添加word-break:break-all;即可

5、文字间距
```
<view style='display: inline-block;'>
  文字1
</view>
<view style='display: inline-block;'>
  文字2
</view>
```

这种在真机上两段文字之间会有空格，修改为:

```
<view style='display: inline-block;'>文字1</view>
<view style='display: inline-block;'>文字2</view>
```
可去除文字间空格
