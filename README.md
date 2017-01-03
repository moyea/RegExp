# RegExp
常用正则表达式

##正则表达式中的特殊字符

* `^` 前缀匹配，匹配字符串必须在最开始
```javascript
/^A/.test('Ana');//=>true
/^A/.test('anA');//=>false
```

* `$` 后缀匹配，匹配的字符串必须在最末尾
```javascript
/A$/.test('aaA');=>true
/A$/.test('Aaa');=>false
```

* `^$` 完全匹配，匹配的字符串必须和给定的表达式完全一致
```javascript
/^AAA$/.test('AAA');//=>true
/^AAA$/.test('AAAA');//=>false
```

## 一些常用表达式
> 金额验证(可以有两位小数): \d+(\.\d{0,2})?  
> 手机号码验证: 1[34578]\d{9}  
> 提取信息中的网络链接:(h|H)(r|R)(e|E)(f|F)\*=\*('|")?(\w|\\|\/|\.)+('|"|\*|>)?  
> 提取信息中的邮件地址:\w+([-+.]\w+)\*@\w+([-.]\w+)\*\.\w+([-.]\w+)\*  
> 提取信息中的图片链接:(s|S)(r|R)(c|C)\*=\*('|")?(\w|\\|\/|\.)+('|"|\*|>)?  
> 提取信息中的IP地址:(\d+)\.(\d+)\.(\d+)\.(\d+)  
> 提取信息中的中国手机号码:(86)\*0\*13\d{9}  
> 提取信息中的中国固定电话号码:(\(\d{3,4}\)|\d{3,4}-|\s)?\d{8}  
> 提取信息中的中国电话号码（包括移动和固定电话）:(\(\d{3,4}\)|\d{3,4}-|\s)?\d{7,14}  
> 提取信息中的中国邮政编码:[1-9]{1}(\d+){5}  
> 提取信息中的中国身份证号码:\d{18}|\d{15}  
> 提取信息中的整数：\d+  
> 提取信息中的浮点数（即小数）：(-?\d\*)\.?\d+  
> 提取信息中的任何数字：(-?\d\*)(\.\d+)?  
> 提取信息中的中文字符串：[\u4e00-\u9fa5]\*  
> 提取信息中的双字节字符串(汉字)：[^\x00-\xff]\*
