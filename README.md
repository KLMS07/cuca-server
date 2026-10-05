# 方块世界 - Minecraft 服务器介绍网站

一个 Minecraft 像素风格的服务器介绍单页网站，使用纯 HTML/CSS/JS 编写，无需构建工具，可直接部署到 GitHub Pages。

## 服务器信息

- **服务器名称**：方块世界
- **服务器号**：3839982
- **QQ交流群**：1081097656
- **服务器类型**：死亡不掉落半规则生存服务器

## 网站功能

- **首页**：服务器概览、核心特色展示、关键信息
- **服务器介绍**：详细介绍、玩法展示、服务器参数
- **游戏规则**：死亡不掉落机制说明、玩家公约
- **联系我们**：服务器号/QQ群一键复制、新手加入指南

## 技术特点

- 单文件 HTML + Hash 路由，四个页面无缝切换
- Minecraft 像素风格设计（像素边框、方块配色、像素字体）
- 完全响应式，适配电脑、平板、手机
- 滚动揭示动画、悬停交互效果
- 纯原生 JS，无任何框架依赖
- 一键复制服务器号和 QQ 群号

## 部署到 GitHub Pages

### 方法一：通过 GitHub 网页界面（推荐新手）

1. 登录 GitHub，点击右上角 **+** → **New repository**
2. 仓库名称填写：`minecraft-server`（或任意名称）
3. 选择 **Public**（公开仓库才能免费使用 GitHub Pages）
4. 勾选 **Add a README file**（可选）
5. 点击 **Create repository**
6. 进入仓库页面，点击 **Add file** → **Upload files**
7. 将本项目的 `index.html` 和 `assets/` 文件夹全部上传
8. 点击 **Commit changes**
9. 进入仓库 **Settings** → 左侧菜单 **Pages**
10. 在 **Source** 中选择 `Deploy from a branch`
11. Branch 选择 `main`，文件夹选择 `/ (root)`，点击 **Save**
12. 等待 1-2 分钟，页面上方会显示你的网站地址，格式为：
    ```
    https://<你的用户名>.github.io/<仓库名>/
    ```

### 方法二：通过 Git 命令行

```bash
# 1. 克隆你的仓库
git clone https://github.com/<你的用户名>/<仓库名>.git
cd <仓库名>

# 2. 将网站文件复制到仓库目录
# （把 index.html 和 assets/ 放进来）

# 3. 提交并推送
git add .
git commit -m "添加 Minecraft 服务器介绍网站"
git push origin main
```

然后按方法一的第 9-12 步在 Settings 中启用 GitHub Pages。

### 自定义域名（可选）

如果有自己的域名，可以在 GitHub Pages 设置页面的 **Custom domain** 中填写，并在域名 DNS 中添加 CNAME 记录指向 `<你的用户名>.github.io`。

## 本地预览

直接用浏览器打开 `index.html` 即可预览，无需任何服务器环境。

如需本地 HTTP 服务器预览：
```bash
# Python 3
python3 -m http.server 8000

# 然后访问 http://localhost:8000
```

## 文件结构

```
minecraft-server/
├── index.html      # 网站主文件（包含所有页面、样式、脚本）
├── assets/         # 图片素材
│   ├── hero.jpg    # 首页背景图
│   ├── base.jpg    # 生存基地图
│   ├── cabin.jpg   # 建筑图
│   ├── isometric.jpg  # 等距世界图
│   └── blocks.jpg  # 方块背景图
└── README.md       # 本说明文件
```

## 修改内容

所有文字内容都在 `index.html` 中，直接用文本编辑器搜索修改即可：

- 修改服务器号：搜索 `3839982`
- 修改 QQ 群号：搜索 `1081097656`
- 修改服务器名称：搜索 `方块世界`
- 修改规则和介绍：找到对应注释区块编辑

---

*本站为玩家自建服务器介绍网站，Minecraft 是 Mojang Studios 的注册商标。*
