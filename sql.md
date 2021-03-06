- 建库，删库

```mysql
CREATE DATABASE 一个数据库;
DROP DATABASE 一个数据库;
```

- 建表，删表

```mysql
CREATE TABLE 一个表 (
  列一 INT,
  列二 INT
);

DROP TABLE 一个表;
```

- 增，删，改，查

```mysql
INSERT 一个表 (列一, 列二) VALUE (1, 2);
INSERT 一个表 (列一, 列二) VALUES (2, 3), (4, 5);

DELETE FROM 一个表
WHERE 列一 = 1;

UPDATE 一个表
SET 列二 = 4
WHERE 列一 = 2；

SELECT * FROM 一个表;
```

- 数据类型

```
# 数字
TINYINT			1
SMALLINT		2
MEDIUMINT		3
INT(INTEGER)	4
BIGINT			8
FLOAT			4
DOUBLE			8
DECIMAL			MAX(M+2,D+2)

# 时间
DATE			3
TIME			3
YEAR			1
DATETIME		8
TIMESTAMP		3

# 字符
CHAR			0-255
VARCHAR			0-65535
TINYBLOB		0-255
TINYTEXT		0-255
BLOB			0-65535
TEXT			0-65535
MEDIUMBLOB		0-16777215
MEDIUMTEXT		0-16777215
LONGBLOB		0-4294967295
LONGTEXT		0-4294967295
```

- 动作

```
CREATE
DROP
INSERT INTO
DELETE
UPDATE
SELECT
```

- 实体

```
DATABASE
TABLE
VIEW
```

- 修饰

```
WHERE
IN
DISTINCT
LIMIT
ORDER BY
GROUP BY
HAVING
```

- 联接与组合

```
(INNER) JOIN ON
LEFT OUTER JOIN ON
UNION
```

- 函数

```
SUM()
AVG()
COUNT()
MAX()
MIN()
```

- 事务

```
START TRANSACTION
ROLLBACK
COMMIT
```

- 约束

```
PRIMARY KEY
UNIQUE
CONSTRAINT
INDEX
```



