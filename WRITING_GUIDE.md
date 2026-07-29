# 如何在 GitHub 网页中发布旅记

本网站使用 Jekyll 和 Markdown，不需要额外后台，也不需要安装软件。

## 发布新文章

1. 打开 `_drafts/travel-post-template.md`。
2. 点击右上角的 **Raw**，复制全部内容。
3. 回到仓库的 `_posts` 文件夹，点击 **Add file → Create new file**。
4. 文件名使用 `年-月-日-英文标题.md`，例如：
   `2026-08-15-oirase-gorge.md`
5. 粘贴模板并修改标题、日期、地点和正文。
6. 点击 **Commit changes**。GitHub Pages 通常会在几分钟内更新网站。

## 添加封面或正文照片

1. 打开 `images` 文件夹。
2. 点击 **Add file → Upload files** 上传照片。
3. 建议使用简短的英文文件名，例如 `oirase-autumn.jpg`。
4. 在文章顶部填写：

```yaml
cover: "/images/oirase-autumn.jpg"
```

正文插图：

```markdown
![奥入濑溪流的秋天]({{ '/images/oirase-autumn.jpg' | relative_url }})
```

## 添加 Google Maps

文章顶部填写：

```yaml
location: "奥入濑溪流"
map_query: "Oirase Gorge, Aomori, Japan"
```

`map_query` 建议使用能在 Google Maps 中准确搜索到的英文地点名称或完整地址。地图会自动出现在文章底部，不需要 Google API Key。

## 暂时不显示地图

删除 `location` 和 `map_query`，或保持为空：

```yaml
location:
map_query:
```
