# 请求替换

把请求替换成请求其它url，配置模式：

	pattern http://host:port:/xxx
	pattern https://host:port:/xxx
	pattern ws://host:port:/xxx
	pattern wss://host:port:/xxx
	
其中，ws[s]和http[s]的请求不能相互替换，pattern参见[匹配方式](../pattern.html)，更多模式请参考[配置模式](../mode.html)。

例子：

把[www.ifeng.com](http://www.ifeng.com/)域名下的请求全部替换成www.aliexpress.com的请求：

		www.ifeng.com www.aliexpress.com
		
用[http://www.ifeng.com](http://www.ifeng.com/)访问HTTPS的[https://www.baidu.com](https://www.baidu.com/)

		http://www.ifeng.com https://www.baidu.com