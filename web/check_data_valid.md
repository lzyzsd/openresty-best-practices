# 数据合法性检测

对用户输入的数据进行合法性检查，避免错误非法的数据进入服务，这是业务系统最常见的需求。很可惜Lua目前没有特别好的数据合法性检查库。

坦诚我们自己做的也不够好，这里只能抛砖引玉，看看大家是否有更好的办法。

我们有这么几个主要的合法性检查场景：

- JSON数据格式
- 关键字段编码为HEX，长度不定
- TABLE内部字段类型

#### JSON数据格式

这里主要是`JSON DECODE`时，可能存在Crash的问题。我们已经在[json解析的异常捕获](json/parse_exception.md)一章中详细说明了问题本身，以及解决方法。这里就不再重复。

#### 关键字段编码为HEX，长度不定

todo list: 

- 到公司补充一下，需要公共模块代码

#### TABLE内部字段类型

todo list: 

- 到公司补充一下，需要公共模块代码

