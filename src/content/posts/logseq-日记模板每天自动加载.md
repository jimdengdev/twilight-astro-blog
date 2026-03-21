---
title: logseq 日记模板每天自动加载
published: 2026-03-21T23:16:00.000+08:00
updated: 2026-03-21T23:16:00.000+08:00
description: logseq 日记模板每天自动加载
cover: https://picsum.photos/800/600?random=3
tags:
  - logseq
  - 日记模板
category: logseq
draft: false
---
# logseq 日记模板每天自动加载

## 前序准备

* logseq mac/pc 版安装完成

## 使用方法

\- 如下图所示，使用 \[[日记模板]] 创建一个 page，然后写下 \`# dailynote\`，

```
# 今日任务
 1. 
 2. 
 3.
# 今日感悟
```

\- 右击点dailynote选择 “创建为模板”，模板名为：daily

\- 在 logseq 设置->常规-> 编辑 config.edn（当前库）

\- 找到 default-templates, 在journals 右边添上模板名 daily，保存重启 logseq 即可生效

```
 :default-templates
 {:journals "daily"}
```
