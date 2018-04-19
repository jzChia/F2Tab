# F2Tab
csv、json、mongo、mysql转tab工具

> 所有数据都必须有一列为空间几何字段，文本类型支持wkt和geojson，mysql支持geometry类型
> csv文件第一行必须为列名，同时有一列为geometry字段，支持wkt和geojson
> mongo数据库的连接字符串格式为：mongodb://user:pwd@localhost:27017/database~collection
> mysql数据库连接字符串为：user:pwd/host:port/db:table

![image](https://github.com/jzChia/F2Tab/blob/master/f2t.jpg)

------------------------------

### 注意事项
> 左侧必须选择空间几何字段，同时必须指定类型
> 可以指定tab字段别名
