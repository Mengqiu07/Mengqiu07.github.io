# 🚀 个人主页极简部署指南（静态版）

> ✅ 模板仓库：`https://github.com/zhengchen1999/Home-Page-Template.git`  
> ✅ 一次配置，后续只需 `git push` 即可更新

### 一、准备仓库

1. 打开模板链接：
    👉 https://github.com/zhengchen1999/Home-Page-Template
2. 点击右上角绿色按钮：
    **“Use this template” → “Create a new repository”**
3. 填写仓库信息：
   - **Repository name：**
     - 如果你想让主页通过
        `https://<你的GitHub用户名>.github.io` 访问，
        仓库名必须是：`<你的GitHub用户名>.github.io`
     - 如果你只想放在子路径访问（比如 `https://<你>.github.io/Home-Page-Template/`），
        可以自定义名称。
4. 点击 **Create repository**。

------

### 二、编辑主页内容

1. 在新创建的仓库里，找到 `index.html` 文件。
2. 点击右上角的 **铅笔图标 ✏️（Edit this file）**。
3. 修改页面文字，例如：
   - 你的姓名、简介、联系方式；
   - 新闻、论文、教育经历等；
4. 点击页面底部的 **Commit changes** 保存修改。

（同理，可打开 `stylesheet.css` 修改颜色、字体等样式。）

---

### 三、开启 GitHub Pages

1. 进入仓库 → 点击上方的 **Settings**。
2. 左侧导航栏选择 **Pages**。
3. 在 **Build and deployment** 区域：
   - Source 选择：**Deploy from a branch**
   - Branch 选择：**main**
   - Directory 选择：**/ (root)**
4. 点击 **Save**。

------

### 四、等待部署完成

几分钟后刷新页面，你会看到提示：

> “Your site is live at https://<你的用户名>.github.io/”

现在即可访问你的主页。

------

### 五、后续更新

- 想修改内容 → 直接网页编辑 `index.html` / `stylesheet.css`。
- 每次点击 **Commit changes** 保存后，网页会自动重新部署。
- 几分钟后刷新主页即可看到新内容。

------

### 六、自定义域名（可选）

1. 在仓库根目录新建文件 `CNAME`。

2. 文件内容只写一行你的域名，例如：

   ```
   xiaomingli.cn
   ```

3. 在域名服务商设置 CNAME 记录，指向：

   ```
   <你的GitHub用户名>.github.io
   ```

4. 回到仓库 → **Settings → Pages → Custom domain**
    填入你的域名，并勾选 **Enforce HTTPS**。

---

### 七、本地预览

1. 将项目下载到本地（推荐使用GitHub Desktop）
2. 使用 VS Code 插件 Live Server 直接打开 `index.html` 实时预览。
