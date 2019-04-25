# F2Tab
csv、json、mongo、mysql,oracle转MapInfo *.tab，Esri shp工具

> 所有数据都必须有一列为空间几何字段，文本类型支持wkt和geojson，mysql,oracle支持geometry类型
> csv文件第一行必须为列名，同时有一列为geometry字段，支持wkt和geojson
> mongo数据库的连接字符串格式为：mongodb://user:pwd@localhost:27017/database~collection
> mysql数据库连接字符串为：user:pwd/host:port/db:table

#### 截图

![image](https://github.com/jzChia/F2Tab/blob/master/f2t.jpg)

------------------------------

### 注意事项
> 左侧必须选择空间几何字段，同时必须指定类型
> 可以指定tab字段别名
> 导出格式为shp时字段长度超过10个字符会被截断


### 使用的python库
```
from Tkinter import *
import tkMessageBox as messageBox
import tkFileDialog as fileDialog
import ScrolledText as sct
import ttk
import osgeo
import osgeo.ogr as ogr
import osgeo.osr as osr
import os
import sys
import datetime
import pymongo
import pymysql
import chardet
import codecs
import csv
import json
import base64
import cx_Oracle
import threading
import time
```
