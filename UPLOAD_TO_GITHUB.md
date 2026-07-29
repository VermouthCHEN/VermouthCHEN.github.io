# 将最小可用版本上传到 GitHub

## 推荐方式：使用 GitHub Desktop

1. 安装并登录 GitHub Desktop。
2. 选择 `File → Clone repository`，克隆 `VermouthCHEN/VermouthCHEN.github.io`。
3. 解压本次交付的 ZIP。
4. 将解压后文件夹里的全部内容复制到本地仓库，允许覆盖同名文件。
5. 在 GitHub Desktop 中确认变更，提交说明可填写：
   `Restore travel blog and add map support`
6. 点击 `Push origin`。

## 只使用 GitHub 网页

需要新增或覆盖的主要文件如下：

- `_config.yml`
- `_layouts/default.html`
- `_layouts/post.html`
- `_sass/_variables.scss`
- `style.scss`
- `index.html`
- `about.md`
- `README.md`
- `WRITING_GUIDE.md`
- `_drafts/travel-post-template.md`
- `_posts/.gitkeep`

对于已有文件，可以打开文件后点击铅笔图标，将交付版本的内容完整覆盖并提交。
对于新文件，可以在对应文件夹中选择 `Add file → Create new file`。

所有文件提交后，打开仓库的 `Actions` 页面检查 GitHub Pages 构建结果。
