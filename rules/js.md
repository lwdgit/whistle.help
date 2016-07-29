# js

往content-type为html或js的响应内容后面追加数据，如果是html，则会自动加上 script 标签在追加到响应内容，如果是js，则会自动追加到js文本后面，这个与[resAppend](resAppend.html)的区别是[resAppend](resAppend.html)不区分类型，对所有匹配的响应都会追加指定的数据，配置模式：

	pattern js://filepath
	
filepath为[Values](http://local.whistlejs.com/#values)里面的{key}或者本地文件，pattern参见[匹配方式](../pattern.html)，更多模式请参考[配置模式](../mode.html)。

例子：

	www.ifeng.com js://{test.js}
	
test.js:

	alert(2);