# ssq01 的博客

本站基于 [gitblog](https://github.com/imuncle/gitblog)，使用 GitHub Issues 作为文章来源，静态页面由 GitHub Pages 托管。

## 发布第一篇文章

首篇文章草稿在 [`drafts/01-hello-world.md`](drafts/01-hello-world.md)。当前仓库尚未启用 Issues；请先在仓库 **Settings → General → Features** 中勾选 **Issues**。要让文章出现在首页，再到 **Issues → New issue**：

1. 将草稿第一行 `# ` 后的文字作为 Issue 标题。
2. 将第一行之后的内容复制到 Issue 正文（不要重复复制标题）。
3. 保持 Issue 为 **Open** 并提交；站点会按 `config.json` 的配置读取开放的 Issues。

本地的草稿文件只是备份，不会自动发布到网站。以后发布文章也采用同样的方法；需要分类时，可在 GitHub 为 Issue 添加标签。

## 站点配置

- `config.json`：仓库、站点标题、简介、导航、友链和页脚图标。
- `images/avatar.jpg` 与 `images/page_background.jpg`：当前头像、背景图，可自行替换。
- `server/gh-oauth-server.php`：模板提供的 OAuth 服务端示例；若启用登录或评论，应使用自己管理的安全服务端。

**安全提醒：**静态网站中的 `config.json` 对访客公开，不能安全保存 OAuth `client_secret`。若当前值是真实凭据，请及时轮换，并将新值仅保存在服务端。原项目许可见 [`LICENSE`](LICENSE)。
