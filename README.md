# yijun-portfolio — 作品集网站

## 文件说明

- `index.html` —— 网站首页。打开时从 `content.json` 实时拉取最新内容（带时间戳跳过缓存），**刷新即更新**。
- `admin.html` —— 内容后台（`/admin.html`）。改完点「☁ 保存并发布」，内容直接写入 `content.json`。
- `content.json` —— 内容数据（作品 + 形象图，图片为 base64 内嵌）。**不要手工改这个文件**，用后台发布。

网站线上地址（WorkBuddy 托管）：https://yijun-portfolio.app.workbuddy.host/

## 日常更新内容

1. 打开 `https://yijun-portfolio.app.workbuddy.host/admin.html`
2. 改内容 → 点「☁ 保存并发布」
3. 打开网站刷新，立刻看到更新。不用再导出、传文件。

## 以后迭代改版

- 改页面结构/样式：编辑 `index.html`，本地用浏览器打开预览，确认后传到 WorkBuddy 覆盖同名文件。
- 改后台功能：编辑 `admin.html`，同样覆盖到 WorkBuddy。
- 内容备份：后台「导出备份 JSON」可随时留底；「导入备份」可恢复。

## Token 说明

后台发布用的是 GitHub fine-grained token（只给本仓库的 Contents 读写权限），只保存在你浏览器的本地。
过期或怀疑泄露时：GitHub 头像 → Settings → Developer settings → Personal access tokens → 吊销旧 token，
重建一个后填进后台「云端连接」即可。
