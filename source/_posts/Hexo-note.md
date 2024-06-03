---
title: Hexo Note
date: 2024-06-02 21:05:45
tags: ['Hexo','Note']
---

## Hexo 資源
- [Hexo 官網](https://hexo.io/zh-tw/)
- [Hexo 英文版教學(YouTube)](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOMJR6D25ishrSedvsguVSm)
- [Hexo 中文版教學(YouTube)](https://www.youtube.com/playlist?list=PLD5dyQmlN6xPqBV0cxO7zAe1C8OmDPqfX)
- [鐵人賽-試著學 Hexo](https://ithelp.ithome.com.tw/users/20119486/ironman/2944)

## 事前準備
- Node.js
- git

安裝完之後可以透過下面指令來確認是否安裝成功
```shell
node -v
git version
npm -v
```

## 安裝Hexo
```shell
npm install -g hexo-cli
```

安裝完之後可以透過下面指令來確認是否安裝成功

```shell
hexo -v
```

## 建立部落格網站
```shell
// 前往要放置部落格網站的資料夾
cd <放置部落格網站的資料夾>

// 建立 Hexo 部落格網站
// <folder> -> 你的網站名稱
hexo init <folder>

// 進入部落格網站的資料夾
cd <folder>

// 安裝需要的套件
npm install
```

## 啟動 Hexo 伺服器
```shell
hexo server
```

## 建立一篇新文章
```shell
hexo new [layout] <title>
```

- 如果沒有提供 layout，則會使用 `_config.yml` 裡面的 `default_layout` 設定。
- 如果 `title` 包含空格，需要用引號括起來。
- 可以使用 `draft` layout 來建立草稿。

## 產生靜態檔案（要部署的內容）
用途：會產生public資料夾，資料夾裡面會放置要部署的內容。
```shell
hexo generate
```

## 清除快取
```shell
hexo clean
```

## 部署內容
用途：將東西部署到 GitHub Pages。
```shell
hexo deploy
```

## Front-matter
- Front-matter 是在 YAML 或 JSON 檔案開頭得一個區塊，用來配置文章的設定。
- Front-matter 使用三個 `-` 來形成區塊（在 YAML 檔案），使用三個 `;` 來形成區塊（在 JSON 檔案）。

### yaml
```yaml
---
title: Hello World
date: 2024/06/01 20:46:25
---
```

### json
```json
"title": "Hello World",
"date": "2024/06/01 20:46:25"
;;;
```
