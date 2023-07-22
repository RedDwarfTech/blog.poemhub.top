---
title: TeX最小化安装
tags:
  - TeX
date: 2023-07-22 17:01:34
---


截止到2023年，TeX Live的完整安装包已经超过了4GB。虽然到2023年磁盘空间已经不是需要特别在意的事情，但是某些场景还是需要最小化安装。比如云上批量部署到时候有时需要更小的镜像来节省镜像下载带宽以及磁盘空间。

## Mac下最小化安装TeX

Mac下最小化安装需要一个小型的分发版(Distribution)Basic TeX,只需要90MB左右的空间，实际可能要更大一些，因为还需要安装一些额外的包。在MacOS下执行以下命令：

```Bash
brew install --cask basictex
```

使用如下命令安装需要的包：

```Bash
sudo tlmgr install ctex
```

## 参考

[1][TUG MacTex文档](https://www.tug.org/mactex/morepackages.html)


