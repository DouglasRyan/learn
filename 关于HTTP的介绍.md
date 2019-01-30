HTTP 是服务器与浏览器交互沟通的协议，是一种约定。
其对浏览器发出的请求和服务器做出的响应进行了规范与标准化。

浏览器发出请求（使用curl命令）
格式
    		1 动词 路径 协议/版本
    		2 Key1: value1
  		2 Key2: value2
    		2 Key3: value3
    		2 Content-Type:application/x-www-form-urlencoded
    		2 Host: www.baidu.com
    		2 User-Agent: curl/7.54.0
    		3 
    		4 要上传的数据
解释
请求最多包含四部分，最少包含三部分。（也就是说第四部分可以为空）	
第一部分由动词 路径 协议/版本组成
动词有 GET POST PUT PATCH DELETE HEAD OPTIONS 等
这里的路径包括 查询参数 但不包括 锚点 ，如果没写，默认为“/”
协议/版本主要是指HTTP协议的版本
第二部分由多个“key,value”键值对构成，
第三部分由一个     回车键       构成
第四部分 为要上传的数据，可以为空
使用Chrome查看请求
f12 查看源代码或者右键 选择查看网页源代码或者使用快捷键 CTRL+U
选择 Network选项
点击第一个文件，查看 Headers 
查看最后一个选项卡 Request Headers
2.服务器做出响应
格式
1 协议/版本号 状态码 状态解释
	2 Key1: value1
	2 Key2: value2
	2 Content-Length: 17931
	2 Content-Type: text/html
	3
	4 要下载的内容
解释
请求包含四部分
第一部分由协议/版本号 状态码 状态解释构成
状态码主要有5种，分别标识不同的响应类型。详情参考 HTTP状态码 中文维基百科https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81
使用Chrome查看响应
f12 查看源代码或者右键 选择查看网页源代码或者使用快捷键 CTRL+U
选择 Network选项
点击第一个文件，查看 Headers 
查看第二个选项卡 Response Headers