---
title: 列出云数据库
---

## 列出云数据库

使用以下命令列出 OSS 对象存储服务

```bash
cf rds ls
```

   <img width="1000" src="/img/1656867218.png">

如果想指定特定属性，可以使用以下参数：

|            参数            |      用途      |
| :------------------------: | :------------: |
|    `-r` 或者 `--region`    |    指定区域    |
| `-i` 或者 -`-DBInstanceID` | 指定数据库 ID  |
|    `-e` 或者 `--engine`    | 指定数据库类型 |

::: warning 注意

* 为了提高程序运行速度，当获取一次结果后，获取的结果会缓存下来，缓存目录为 `~/.cf/cache`
* 如果不想使用缓存数据，可以在执行命令的时候加上 `--flushCache` 参数

::: 

<Vssue />

<script>
export default {
    mounted () {
      this.$page.lastUpdated = "2022年7月4日"
    }
  }
</script>