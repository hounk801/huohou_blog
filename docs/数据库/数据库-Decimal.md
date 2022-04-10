当必须保持精确度时，例如货币数据，则使用此类型

在列声明中，可以（并且通常）指定精度和小数位数
```
column_name  DECIMAL(P,D);
```
在上面的语法中：

P是表示有效数字数的精度。 P范围为1〜65。
D是表示小数点后的位数。 D的范围是0~30。MySQL要求D小于或等于(<=)P。

与INT数据类型一样，DECIMAL类型也具有UNSIGNED和ZEROFILL属性。 

如果使用UNSIGNED属性，则DECIMAL UNSIGNED的列将不接受负值。

如果使用ZEROFILL，MySQL将把显示值填充到0以显示由列定义指定的宽度。 另外，如果我们对DECIMAL列使用ZERO FILL，MySQL将自动将UNSIGNED属性添加到列。

