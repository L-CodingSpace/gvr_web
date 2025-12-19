# Gen-ViRe: A Generative Visual Reasoning Benchmark

这是 Gen-ViRe 项目的官方网站。

## 🌐 在线访问

**网站将部署在:** `https://YOUR_USERNAME.github.io/YOUR_REPO/`

## 🚀 快速部署（接下来的步骤）

### 步骤 1: 创建 GitHub 仓库

1. 访问 https://github.com/new
2. 填写仓库信息：
   - **Repository name**: `gen-vire`（或其他你喜欢的名字）
   - **Description**: `Gen-ViRe: A Generative Visual Reasoning Benchmark`
   - **Public** ✅ (必须是公开的才能使用免费的 GitHub Pages)
   - ⚠️ **不要**勾选 "Add a README file"
3. 点击 "Create repository"

### 步骤 2: 推送到 GitHub

创建仓库后，GitHub 会显示一个页面。在终端中执行以下命令（替换为你的实际信息）：

```bash
cd /Users/ming/Desktop/github_page/gvr_web
git remote add origin https://github.com/YOUR_USERNAME/gen-vire.git
git branch -M main
git push -u origin main
```

**示例（如果你的 GitHub 用户名是 `john`）：**
```bash
git remote add origin https://github.com/john/gen-vire.git
git branch -M main
git push -u origin main
```

### 步骤 3: 启用 GitHub Pages

1. 进入你的 GitHub 仓库页面
2. 点击 **Settings** (设置) 标签
3. 在左侧菜单中找到 **Pages**
4. 在 "Build and deployment" 部分：
   - **Source**: Deploy from a branch
   - **Branch**: 选择 `main` 和 `/ (root)`
   - 点击 **Save**
5. 等待 1-2 分钟，页面会显示你的网站地址

### 步骤 4: 访问你的网站！

你的网站地址将是：
```
https://YOUR_USERNAME.github.io/gen-vire/
```

## 📁 项目结构

```
gvr_web/
├── index.html              # 主页面（已从 website.html 重命名）
├── figs/                   # 研究图表和图片
├── two_row_image/          # 任务展示图片
├── videos/                 # 视频演示文件
│   ├── 1/                  # Sora-2 对比视频
│   └── 2/                  # 7 模型对比视频
├── DEPLOYMENT_GUIDE.md     # 详细部署指南
└── README.md               # 本文件
```

## 🔄 更新网站内容

当你需要更新网站时，在 `gvr_web` 目录下执行：

```bash
git add .
git commit -m "描述你的修改"
git push
```

GitHub Pages 会自动重新部署（通常需要 1-2 分钟）。

## ✅ 已完成的准备工作

- ✅ 将 `website.html` 重命名为 `index.html`
- ✅ 初始化 Git 仓库
- ✅ 添加并提交所有文件（48 个文件）
- ✅ 检查视频文件大小（62MB，符合 GitHub 限制）

## 📊 文件统计

- 总文件数: 48
- HTML 文件: 1
- 图片文件: 38
- 视频文件: 8（总大小 62MB）

## 🆘 需要帮助？

查看 `DEPLOYMENT_GUIDE.md` 获取详细的部署说明和常见问题解决方案。

## 📄 论文信息

- **标题**: Can World Simulators Reason? Gen-ViRe: A Generative Visual Reasoning Benchmark
- **arXiv**: https://arxiv.org/pdf/2511.13853
- **GitHub Code**: https://github.com/L-CodingSpace/GVR

---

Made with ❤️ by the Gen-ViRe Team


