# MongoDB

MongoDB 学习笔记

<!-- HACK: Github上无法显示目录树 -->

[TOC]

## Install

1. MongoDB
2. MongoDB Compass
3. MongoDB Tool

## Import and Export

### Import

```bash
cd '.\1.Import&Export\'
mongoimport --db test --type json products.json
```

然后在 Compass 中可以查看到导入的数据

### Export

```bash
cd '.\1.Import&Export\'
mongoexport -d test -c products -o pro.json
nvim pro.json
```

## 基本操作

- 查看所有数据库

  ```bash
  show dbs
  ```

- 创建数据库

  ```bash
  use example
  ```

  > NOTE：如果里面没有数据，并不会真正的创建。在图形化管理工具中并不会显示该数据库

- 查看当前使用的数据库

  ```bash
  db
  ```

- 插入数据

  ```bash
  doc = {"title":"A","content":"第一个数据"}
  db.some.insertOne(doc)
  ```

## Collections 简介与基础操作

- 切换到 test 数据库

  ```bash
  use test
  ```

- 清屏

  ```bash
  cls
  ```

- 显示当前数据库中的 Collections

  ```bash
  show collections;
  ```

- 查询所有数据

  ```bash
  db.products.find();
  ```

