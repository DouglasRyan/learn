iframe 标签
嵌套页面

<iframe src="https://www.baidu.com" name="xxx"></iframe>
a 标签
跳转页面（HTTP GET 请求）

属性见 MDN：https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/a

form 标签
跳转页面（HTTP POST 请求）

属性见 MDN：https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/form

input / button
区别：是否为「空标签」

input 的属性见：https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/Input
button 的属性见：https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/button

table 标签示例
用于展示数据

属性见：https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/table

知识点：

空标签
可替换标签
全局属性
display 不止 3 种

1、HTML代码
    布局：横向--纵向
    标签：
2、标签——iframe / a / form / table
    iframe ——嵌套页面
        frameborder="0"
        name属性——target属性使用（a）name
    a ——超链接
        download
        target ——"_self/_blank_/parent/_top"
        href 
            无协议、路径/锚点/查询参数/伪协议（不动/执行js——JavaScript：；）
    form
        必须有提交按钮
        input——button（type）
        button（唯一）——submit
        技巧：label包含input
    table
        thead——tr/th/td
        tobody
        tfooter
        col-colgroup
    