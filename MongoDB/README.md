# MongoDB

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
然后在Compass中可以查看到导入的数据

### Export
```bash
cd '.\1.Import&Export\'
mongoexport -d test -c products -o pro.json
nvim pro.json
```
