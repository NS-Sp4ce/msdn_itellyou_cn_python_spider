# msdn_itellyou_cn_spider_python
msdn.itellyou.cn爬虫python版【需要mysql】

# 数据库配置
*conn=pymysql.connect(host='localhost', port=3306, user='root', password="", db='smzdm', charset='utf8')*

> host:数据库IP
>
> port：端口
>
> user:用户名
>
> password:密码
>
> db:数据库名称
>
> charset:数据库编码

# 创建数据表（默认为itellyou_copy1）

```
use smzdm;
DROP TABLE IF EXISTS `itellyou_copy1`;
CREATE TABLE `itellyou_copy1`  (
  `menu` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `name` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `country` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `version` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `FileName` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `SHA1` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `dt` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `PostDataString` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL,
  `DownLoad` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci NULL DEFAULT NULL
) ENGINE = InnoDB CHARACTER SET = utf8 COLLATE = utf8_general_ci ROW_FORMAT = Dynamic;
```

# 需要安装的模块
pymysql、BeautifulSoup
