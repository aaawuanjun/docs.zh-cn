# reverse

## 功能

将字符串/数组反转，返回的字符串/数组的顺序和源字符串/数组的顺序相反。

## 语法

`reverse(param)`

## 参数说明

`param`：需要反转的字符串/数组。支持的数据类型为 VARCHAR、CHAR、ARRAY。

## 返回值说明

返回的数据类型与 `param` 一致。

## 注意事项

* 如果 `param` 是数组类型，返回数组中的元素类型和 `param` 中的元素类型一致。
* 如果 `param` 是数组类型，只支持一维数组。
* 如果 `param` 是数组类型，数组中元素类型不允许为 `DECIMAL`。

## 示例

反转字符串。

```Plain Text
MySQL > SELECT REVERSE('hello');
+------------------+
| REVERSE('hello') |
+------------------+
| olleh            |
+------------------+

MySQL > SELECT REVERSE('你好');
+------------------+
| REVERSE('你好')  |
+------------------+
| 好你             |
+------------------+
```

反转数组。

```Plain Text
MYSQL> SELECT REVERSE([4,1,5,8]);
+--------------------+
| REVERSE([4,1,5,8]) |
+--------------------+
| [8,5,1,4]          |
+--------------------+
```

## keyword

REVERSE, ARRAY
