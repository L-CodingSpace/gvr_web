# 🚀 GitHub Pages 部署指南

## 当前进度
✅ 已将 website.html 重命名为 index.html  
✅ 已初始化 Git 仓库

## 接下来的步骤

### 1. 添加并提交文件到本地仓库

```bash
cd /Users/ming/Desktop/github_page/gvr_web
git add .
git commit -m "Initial commit: Gen-ViRe website"
```

### 2. 在 GitHub 上创建新仓库

1. 访问 https://github.com/new
2. 仓库名称建议: `gen-vire` 或 `gvr-web`
3. 选择 **Public** (公开)
4. **不要**勾选 "Add a README file"
5. 点击 "Create repository"

### 3. 连接本地仓库到 GitHub

复制 GitHub 给你的仓库地址，然后执行（将 `YOUR_USERNAME` 和 `YOUR_REPO` 替换为实际值）:

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git branch -M main
git push -u origin main
```

### 4. 启用 GitHub Pages

1. 进入你的 GitHub 仓库页面
2. 点击 **Settings** (设置)
3. 在左侧菜单找到 **Pages**
4. 在 "Source" 下选择:
   - Branch: `main`
   - Folder: `/ (root)`
5. 点击 **Save**

### 5. 等待部署完成

- 通常需要 1-2 分钟
- 部署完成后，你会看到一个绿色提示框，显示网站地址
- 地址格式: `https://YOUR_USERNAME.github.io/YOUR_REPO/`

## 📝 注意事项

### 文件大小限制
GitHub Pages 有一些限制：
- 单个文件不超过 100MB
- 建议整个仓库不超过 1GB
- 视频文件可能比较大，检查 `videos` 文件夹大小

### 检查视频文件大小
```bash
du -sh videos/
```

如果视频文件太大（>50MB），建议：
1. 压缩视频
2. 或上传到视频托管服务（如 YouTube, Vimeo）
3. 或使用 Git LFS (Large File Storage)

### 自定义域名（可选）
如果你有自己的域名，可以在 GitHub Pages 设置中添加自定义域名。

## 🔄 更新网站

每次修改后，使用以下命令更新：

```bash
git add .
git commit -m "更新说明"
git push
```

GitHub Pages 会自动重新部署。

## 🆘 常见问题

### 问题: 404 错误
- 确保文件名是 `index.html`（已完成✅）
- 确保 GitHub Pages 已启用
- 等待几分钟让部署完成

### 问题: 图片/视频无法显示
- 检查文件路径是否正确（相对路径）
- 确保所有资源文件都已提交到仓库
- 检查文件名大小写（Linux 区分大小写）

### 问题: 视频文件太大
```bash
# 检查大文件
find . -type f -size +50M

# 使用 Git LFS（如果需要）
git lfs install
git lfs track "*.mp4"
git add .gitattributes
```

## 📧 分享你的网站

部署完成后，你可以分享这个地址：
```
https://YOUR_USERNAME.github.io/YOUR_REPO/
```

享受你的在线网站！🎉

