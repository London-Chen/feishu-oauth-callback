# Obsidian Feishu Sync - OAuth Callback

这是 Obsidian Feishu Sync 插件的 OAuth 授权回调页面。

## 部署到 GitHub Pages

1. Fork 或克隆此仓库
2. 进入仓库设置 (Settings)
3. 找到 "Pages" 选项
4. 在 "Source" 中选择 `main` 分支和 `/` (root) 目录
5. 点击 Save
6. 等待几分钟后，你的页面将部署到 `https://yourusername.github.io/repo-name/oauth-callback.html`

## 配置飞书应用

在飞书开放平台的应用设置中：

1. 进入「安全设置」

2. 在「重定向 URL」中添加：

   ```
   https://yourusername.github.io/repo-name/oauth-callback.html
   ```

3. 保存并发布应用版本

## 配置 Obsidian 插件

在 Obsidian 的 Feishu Sync 插件设置中：

1. 将「OAuth 回调 URL」设置为你的 GitHub Pages 地址
2. 选择「手动（粘贴授权码）」模式
3. 点击「授权」按钮
4. 在浏览器中完成授权后，复制显示的授权码
5. 返回 Obsidian 粘贴授权码

## 隐私说明

此回调页面完全在浏览器本地运行，不会向任何服务器发送你的授权码。所有代码都是开源的，你可以查看 `oauth-callback.html` 的源代码。
