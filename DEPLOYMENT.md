# 骆驼奶商店网站部署指南

本文档提供了将骆驼奶商店网站部署到公网的详细步骤，使不在同一局域网的人也能访问。

## 方法一：使用GitHub Pages部署（推荐）

### 前提条件
- 拥有GitHub账号
- 安装Git

### 部署步骤

1. 在GitHub上创建一个新的仓库，例如`camel-milk-store`

2. 在本地初始化Git仓库并推送到GitHub
   ```bash
   git init
   git add .
   git commit -m "初始化骆驼奶商店网站"
   git branch -M main
   git remote add origin https://github.com/你的用户名/camel-milk-store.git
   git push -u origin main
   ```

3. 在GitHub仓库设置中启用GitHub Pages
   - 进入仓库 -> Settings -> Pages
   - Source选择`main`分支
   - 点击Save

4. 等待几分钟后，你的网站将会在以下地址可用：
   `https://你的用户名.github.io/camel-milk-store/`

## 方法二：使用Netlify部署

1. 注册Netlify账号：https://www.netlify.com/

2. 点击"New site from Git