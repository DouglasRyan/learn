1、万维网来历
    服务器+浏览器+网页
    
2、HTTP+HTML+URL

3、curl命令
    curl -s -v -H "Frank: xxx" -- "https://www.baidu.com"
    curl -X POST -s -v -H "Frank: xxx" -- "https://www.baidu.com"

4、请求与响应
    浏览器负责发起请求
    服务器在 80 端口接收请求
    服务器负责返回内容（响应）
    浏览器负责下载响应内容

    请求格式
        1 动词 路径 协议/版本
        2 Key1: value1
        2 Key2: value2
        2 Key3: value3
        2 Content-Type: application/x-www-form-urlencoded
        2 Host: www.baidu.com
        2 User-Agent: curl/7.54.0
        3 
        4 要上传的数据
        请求最多包含四部分，最少包含三部分。（也就是说第四部分可以为空）
        第三部分永远都是一个回车（\n）
        动词有 GET POST PUT PATCH DELETE HEAD OPTIONS 等
        这里的路径包括「查询参数」，但不包括「锚点」
        如果你没有写路径，那么路径默认为 /
        第 2 部分中的 Content-Type 标注了第 4 部分的格式

5、chrome用network查看请求和响应

6、DNS和hosts
    DNS域名服务器
    IP
    c:\windows\system32\drivers\etc/hosts