> 一个小而快的GBK库,支持浏览器

### 等点如下：
1. 编码表是经过简单压缩的，只有不到60k。
	> 正常的编码表最少要到200K左右
2. 通过二分法查询，比通过map对像查询要快很多。
3. 不包含GBK自定义（扩展）码区。

> 内存占用和一般的gbk库差不多，但加载时会解压编码表，加载时间稍多

## API
### GBK.encode({byteArry}) 解码GBK编码的 `byteArray` 返回字符串

### GBK.decode({string})