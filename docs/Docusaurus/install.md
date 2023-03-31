---
sidebar_position: 1
---

# Install

## 版本需求

要安裝 Docusaurus 首先需要安裝 Node.js，版本需求為 16.14 或以上。

## 建立專案

然後只要在終端機輸入以下指令，`my-website` 可以自定義專案名稱：

```bash
npx create-docusaurus@latest my-website classic
```

## 專案結構

然後用任一個編輯器打開專案，可以看到你的專案結構如下：

```
my-website
├── blog
│   ├── 2019-05-28-hola.md
│   ├── 2019-05-29-hello-world.md
│   └── 2020-05-30-welcome.md
├── docs
│   ├── doc1.md
│   ├── doc2.md
│   ├── doc3.md
│   └── mdx.md
├── src
│   ├── css
│   │   └── custom.css
│   └── pages
│       ├── styles.module.css
│       └── index.js
├── static
│   └── img
├── docusaurus.config.js
├── package.json
├── README.md
├── sidebars.js
└── yarn.lock
```

- /blog/ - 如果有需要使用 blog 的話，這裡包含 blog 的 Markdown 文件。如果沒有要使用這個路徑，可以刪除此目錄，或在設置路徑選項後更改其名稱。
- /docs/ - 包含 docs 的 Markdown 文件。在 sidebars.js 中自定義文檔側邊欄的順序。一樣如果沒有要使用這個路徑，可以刪除此目錄，或在設置路徑選項後更改其名稱。有關詳細信息，請參閱文檔指南。
- /src/ - 非文檔類文件，如頁面或自定義 React 組件。嚴格來說，您不一定要將非文檔類文件放在這裡。但將它們放在一個集中的目錄中可以讓代碼檢查或處理更加方便。
- /src/pages - 此目錄中的任何 JSX/TSX/MDX 文件都會轉換為網站頁面。有關詳細信息，請參閱頁面指南。
- /static/ - 靜態目錄。此處的任何內容都將複製到最終構建目錄的根目錄中。
- /docusaurus.config.js - 包含站點配置的配置文件。這相當於 Docusaurus v1 中的 siteConfig.js。
- /package.json - Docusaurus 網站是一個 React 應用程序。您可以安裝和使用任何 npm 套件。
- /sidebars.js - 用於 docs，以指定側邊欄 docs 的順序。

## 預覽

在終端機輸入以下指令，即可在本地預覽網站：

```bash
npm run start
```