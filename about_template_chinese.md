#NUBBS模板解答
# Introduction #

Python版本的NUBBS模板疑问解答

# Details #

Q:模板里如何放置变量：
A:用两个花括号和一个空格括起来，例如：“ {{ variable }} 　”。
又如：“{{ section.title }}　”，表示section对象的title属性值，“.”用来分隔对象（写在“.”的左边）和属性（写在右边）。
再如：“{{ name|lower }}　”表示把name变量转成小写。
例4：“ {{ text|escape|linebreaks }}　”是把text变量转义并在每一行加上html的p标签（<p>）<br>
例5：“{{ bio|truncatewords:30 }}　”只保留bio前30个字符。冒号后表示函数的变量。<br>
例6：“{{ list|join:", " }}　”把名为list的列表对象各个对象用逗号和空格连接。<br>
例7：“{{ value|default:"defaultvalue" }}　”，如果value为空或false，则显示defaultvalue。<br>
例8：“{{ value|striptags }}　”去掉html和xhtml标签，留下纯文本。<br>
例9：“{{ value|length }}　”，显示对象的长度或元素的个数。