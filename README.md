#jquery.raty.js评分插件
    jQuery Raty这是一个能够自动生成可定制的星级评分jQuery插件。可以自定义图标，创建各种评级组合，星星数量，每一颗星星的注释，可以在当一个星星被点击时的加回调函数。
####下载地址：https://github.com/wbotelhos/raty

##兼容性
* ie6+

##样例：

###1、使用步骤
* 引入js文件（jquery-1.9.1.min.js，jquery.raty.js）
```javascript
<script type="text/javascript" src="javascript/jquery-1.9.1.min.js"></script>
<script type="text/javascript" src="javascript/jquery.raty.js"></script>
```
* 在页面上添加代码
```javascript
<div id="raty" data-number="5" data-path="images/raty"></div>
<div id="ratydesc" class="hint"></div>
```

###2、demo
* [PDF文件阅读demo](http://192.168.14.97:8080/acc/plugin/raty)

##配置和API
###1、页面配置
```javascript
$('#raty').raty({
    path: function() {
        return this.getAttribute('data-path');//图片路径
    },
    number: function() {
        return $(this).attr('data-number');//星星数量
	},
	starOn: 'star-smile-gorgeous.png',//激活星星图标
	starOff: 'star-smile-off.png',//未激活星星图标
	halfShow : 'false',//是否显示半颗星星
	hints: ['很差', '一般', '好', '很好', '非常好'],//等级的内容
	target: '#ratydesc',//评分等级显示的div
	targetType: 'hint',//评分等级显示的div
	targetKeep: true,//固定显示评分结果
	targetText: '请打分'//评分结果默认显示文字
});
```

###2、API
* [jquery.raty.js的API详细参数地址](http://bookshadow.com/weblog/2014/08/16/jquery-raty-star-plugin/)







