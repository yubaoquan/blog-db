# blog-db

Data source of some-blog

## centOs 安装 mySql

[参考链接](https://www.mysqltutorial.org/install-mysql-centos/)

## 问题解决方法

### 连不上mysql

报错:

```text
error Error: ER_NOT_SUPPORTED_AUTH_MODE: Client does not support authentication protocol requested by server; consider upgrading MySQL client
```

解决:

```sql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'xxxxxx';
```

[参考链接: 解决Node.js mysql客户端不支持认证协议引发的“ER_NOT_SUPPORTED_AUTH_MODE”问题](https://waylau.com/node.js-mysql-client-does-not-support-authentication-protocol/)

[参考链接2: stackoverflow](https://stackoverflow.com/questions/50093144/mysql-8-0-client-does-not-support-authentication-protocol-requested-by-server)
