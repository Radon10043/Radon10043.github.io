---
layout: post
title: Python打包第三方库并离线安装的指令
description: >
  三条命令搞定Python第三方库的打包与离线安装，适用于无法连接外网的环境。
categories: [Tech]
tags: [Python, pip]
---

生成requirements.txt

```bash
pip freeze > /path/to/requirements.txt
```

根据requirements.txt里的内容对第三方库进行打包

```bash
pip download -d package -r /path/to/requirements.txt
```

在其他电脑上进行离线安装

```bash
pip install --find-links=/path/to/package -r /path/to/requirements.txt
```
