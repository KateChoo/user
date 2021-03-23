# 基本的 SQL 指令

## 登入 mysql

```bash
mysql -u root -p
```

## 秀出資料庫

```bash
SHOW DATABASES;
```

## 建立新的資料庫

```bash
CREATE DATABASE [mysqldb name];
```

## 使用該資料庫

```bash
USE website;
```

## 建立新的 table

```bash
mysql> CREATE TABLE user(
    -> id BIGINT AUTO_INCREMENT,
    -> name VARCHAR(255) NOT NULL,
    -> username VARCHAR(255) NOT NULL,
    -> password VARCHAR(255) NOT NULL,
    -> time DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
    -> PRIMARY KEY(id)
    -> );
```

## 刪除 table

```bash
DROP TABLE tablename
```

## 刪除 database

```bash
DROP DATABASE databasename
```

## 展示 column

```bash
SHOW COLUMNS FROM test;
```

1. SHOW DATABASES;
   <img src="img/1.png" alt="SHOW DATABASES;"/>
2. USE website;
   <img src="img/2.png" alt="USE website;"/>
3. SHOW TABLES;
   <img src="img/3.png" alt="SHOW TABLES;"/>
4. SHOW COLUMNS FROM user;
   <img src="img/4.png" alt="SHOW TABLES;"/>
5. INSERT user1
   <img src="img/5.png" alt="SHOW TABLES;"/>
6. SELECT \* FROM user;
   <img src="img/6.png" alt="SHOW TABLES;"/>
7. SELECT COUNT(\*) FROM user;
   <img src="img/7.png" alt="SHOW TABLES;"/>
8. SELECT username FROM user ORDER BY time DESC;
   <img src="img/8.png" alt="SHOW TABLES;"/>
9. SELECT \* FROM user WHERE id BETWEEN 2 AND 4 ORDER BY time DESC;
   <img src="img/9.png" alt="SHOW TABLES;"/>
10. SELECT \* FROM user WHERE username = 'ply' AND password = 'ply';
    <img src="img/10.png" alt="SHOW TABLES;"/>
11. UPDATE user
    <img src="img/11.png" alt="SHOW TABLES;"/>
