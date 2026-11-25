# Leisurely · Automation Build Journal Vol.07

天行健双语品牌页，单文件、图片全内嵌，可直接作为 GitHub Pages 首页。

## 最快上线（浏览器，3 分钟）

1. 登录 GitHub，右上角 **+ → New repository**。
2. 仓库名填 `automation-vol7`，选 **Public**，点 **Create repository**。
3. 进仓库，点 **Add file → Upload files**，把本目录的 `index.html` 和 `.nojekyll` 一起拖进去，点 **Commit changes**。
4. 打开 **Settings → Pages**：
   - Source 选 **Deploy from a branch**
   - Branch 选 **main**，目录选 **/ (root)**
   - 点 **Save**
5. 等 1–2 分钟，页面地址是：

   `https://你的用户名.github.io/automation-vol7/`

如果仓库名直接用 `你的用户名.github.io`，地址就是 `https://你的用户名.github.io/`。

## 更新版本

把新的 `index.html` 重新上传覆盖，Commit 后 Pages 会自动重新部署。

## 可选：命令行

```bash
git init
git add index.html .nojekyll
git commit -m "Leisurely Vol.07"
git branch -M main
git remote add origin https://github.com/你的用户名/automation-vol7.git
git push -u origin main
```

然后在 Settings → Pages 里选 `main` / root。

## 说明

- 页面是自包含单文件，约 3.64 MB，不需要额外图片目录。
- GitHub 网页上传单文件上限 25 MB，这个文件在范围内。
- GitHub Pages 免费版软限制：站点 1 GB、月流量 100 GB、每小时 10 次构建；个人品牌页足够。
- 自定义域名：Settings → Pages → Custom domain，填域名后在 DNS 加 CNAME 记录。
- 页面里的中英切换会记住访客选择；`?lang=zh` 可直接打开中文。
