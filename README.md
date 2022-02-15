# Koa2_Mysql_Demo

node+koa2+mysql

### 创建数据库

登录数据库

```
$ mysql -u root -p
```

创建数据库

```
$ create database nodesql;
```

使用创建的数据库

```
$ use nodesql;
```

> database: nodesql tables: users posts comment (已经在 lib/mysql 建表)

```js
|   users     |   posts      |   comment   |
| :---------: | :----------: | :---------: | --- |
|     id      |      id      |     id      |
|    name     |     name     |    name     |
|    pass     |    title     |   content   |
|  avator     | content      |   moment    |
|   moment    |    md        |    postid   |
|      -      |   uid        |   avator    |
|      -      |  moment      |      -      |
|       -     | comments     |      -      |     |
|       -     |    pv        |      -      |     |
|       -     |  avator      |      -      |     |
```

- id 主键递增
- name: 用户名
- pass：密码
- avator：头像
- title：文章标题
- content：文章内容和评论
- md：markdown 语法
- uid：发表文章的用户 id
- moment：创建时间
- comments：文章评论数
- pv：文章浏览数
- postid：文章 id

```
$ git clone https://github.com/otxwg/Koa2_Mysql_Demo.git
```

```
$ cd Koa2_Mysql_Demo
```

```
$ cnpm i supervisor -g
```

```
$ cnpm i
```

```
$ npm run dev(运行项目)
```

```
$ npm test(测试项目)
```
