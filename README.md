# jquery-fixed-qq
该悬浮QQ在线客服插件一款很实用的功能，基本每个企业网站都需要，能及时解决网站访客的提问，转化成企业的客户 。

![悬浮QQ在线客服插件](http://7xp00j.com1.z0.glb.clouddn.com/static/images/2eb1da14-e5f4-4a89-ae1d-1a1205f722fa.png)

提供6种不同颜色的皮肤以及2个完全不同风格的皮肤给用户选择。解决了之前第一版本在Chrome浏览器中，点击收缩时悬浮窗口不显示的BUG。另外，还增加了几个参数，让该插件的在应对更多需求时更具灵活性。
需要引用的文件：

**1、CSS**
``` css
<link rel="stylesheet" type="text/css" href="css/service.css"/>
```
**2、jQuery**
``` javascript
<script type="text/javascript" src="js/jquery-1.4.4.min.js"></script>
<script type="text/javascript" src="js/jquery.fixed.1.5.1.js"></script>
```
**3、jQuery的调用**
``` javascript
<script language="javascript">
$(window).load(function(){
	$("#fixedBox2").fix({
		position	: "left",
		horizontal	: 50,
		vertical	: null,
		halfTop		: false,
		minStatue	: false,
		hideCloseBtn	: false,
		skin		: "gray",
		showBtnWidth	: 28,
		contentBoxWidth : 154,
		durationTime	: 600 
	});
	
	$("#fixedBox").fix({
		position	: "right",
		horizontal	: 0,
		vertical	: 100,
		halfTop		: true,
		minStatue	: false,
		hideCloseBtn	: false,
		skin		: "blue",
		showBtnWidth	: 28,
		contentBoxWidth	: 154,
		durationTime	: 1000
	});	
});
</script>
 ```

**可设置项有：**

1.悬浮的位置，右侧还是左侧

2.离浏览器侧边的水平方向距离

3.离浏览器顶部的垂直方向距离

4.是否垂直居中

5.是否默认显示最小化

6.是否隐藏关闭按钮

7.选择哪种风格皮肤

8.显示按钮的宽度

9.悬浮窗口的宽度

10.滑动的速度
