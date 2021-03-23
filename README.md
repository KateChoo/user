# 基本的 SQL 指令

##登入 mysql

```bash
mysql -u root -p
```

1. SHOW DATABASES;
   <img src="img/1.png" alt="SHOW DATABASES;"/>
2. USE website;
3. SHOW TABLES;
4. SHOW COLUMNS FROM user;
5. INSERT user1
6. SELECT \* FROM user;
7. SELECT COUNT(\*) FROM user;
8. SELECT username FROM user ORDER BY time DESC;
9. SELECT \* FROM user WHERE id BETWEEN 2 AND 4 ORDER BY time DESC;
10. SELECT \* FROM user WHERE username = 'ply' AND password = 'ply';
11. UPDATE user
