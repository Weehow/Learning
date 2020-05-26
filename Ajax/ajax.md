XAMMP [傻瓜化的安装PHP](https://www.apachefriends.org/download.html)

JSONLint 校验json格式, jsonline.com

/* JSON的两种解析方式 */
var jsondata = '{"staff": [{"name" : "张三","age" : 30},{"name" : "李四","age" : 20},{"name" : "王五","age" : 35} ]}';
var jsonobj = eval('(' + jsondata + ')');
alert(jsonobj.staff[0].name); <!-- 不严谨 -->

var jsondata = '{"staff": [{"name" : "张三","age" : 30},{"name" : "李四","age" : 20},{"name" : "王五","age" : 35} ]}';
var jsonobj = JSON.parse(jsondata);
alert(jsonobj.staff[0].name); <!-- 多用 -->

{
	"success": true,  /* 请求是否成功*/
	"msg": "xxx",	<!-- 返回错误信息 -->
	"data": "xxx"
}