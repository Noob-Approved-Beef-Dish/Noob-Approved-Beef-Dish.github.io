# website

牛肉饼的个人网站 —— 单文件、零依赖、纯静态。

## 本地预览

直接双击 `index.html` 就能看，不用装任何东西。

文件就三个：`index.html`（全部内容）、`avatar.jpg`（头像，也当网站图标）、`.nojekyll`（别删）。

想用本地服务器预览（更像线上环境）：

    python -m http.server 8000

然后打开 http://127.0.0.1:8000

## 部署到 GitHub Pages

### 方式 A · 用户站点（推荐，地址最短）

1. 新建仓库，名字**必须是** `Noob-Approved-Beef-Dish.github.io`
2. 把 `index.html` 推到 `main` 分支
3. 等 1 分钟，访问 https://noob-approved-beef-dish.github.io

### 方式 B · 项目站点

1. 新建仓库（比如 `website`），把文件推上去
2. 仓库 Settings → Pages → Source 选 `Deploy from a branch`
3. Branch 选 `main` / 目录选 `/ (root)` → Save
4. 等 1 分钟，访问 `https://noob-approved-beef-dish.github.io/website/`

## 怎么改内容

只改 `index.html` 一个文件。结构是这样：

    <h2>whoami</h2>      自我介绍
    <h2>projects</h2>    项目（一行一个 <tr>）
    <h2>skills</h2>      技能
    <h2>now</h2>         最近在干嘛
    <h2>links</h2>       外链

配色在文件顶部的 `:root` 里改，变量名一看就懂。

## 隐私提醒

- **不要**写真实姓名、具体住址、学校班级、手机号
- 邮箱建议留空，或者只放 GitHub 联系方式
- 这里写的所有东西都是**公开**的，搜索引擎会收录
