# BDUSS获取

## workers

在 <https://workers.cloudflare.com> 新建一个workers，将 `workers.js` 的内容复制粘贴就完成了

- 可以设置环境变量或者取消注释设置 `ORIGIN`

## php

- 可以取消注释设置 `$origin`

## 示例

`/docs/index.html` 是演示站 <https://bduss.ailand.date> 的源码，要直接使用需要修改或者删除下述几项

- `L82` 及 `L83` Google analytics 相关
- `L98` api地址
- \* 使用php需要修改 `L99` 的 `workersMode` 至 `false`

## 环境要求

仅限 PHP 版有要求，workers 版直接部署

```txt
php 7.x
php-curl
```

## 其他

关于 Google analytics 可以参考 [SukkaW/cloudflare-workers-async-google-analytics](https://github.com/SukkaW/cloudflare-workers-async-google-analytics)
