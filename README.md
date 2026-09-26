# 法律文档网页（发布用）

> ✅ 已发布：https://kawhijimmy-cpu.github.io/driftmaster-legal/ （2026-09-27 验证 6 个页面均返回 200）

这个文件夹里的 5 份文档就是要发布成公网链接的内容。目录名与旧站保持一致，所以以后换域名只需要改域名，不用改路径。

发布后的地址形如：

- `https://<域名>/privacy-policy/`
- `https://<域名>/terms-of-service/`
- `https://<域名>/data-deletion/`
- `https://<域名>/children-privacy/`
- `https://<域名>/third-party-sharing/`

## 发布到 GitHub Pages（推荐，免费）

1. 登录你的 GitHub 账号 → **New repository**
   - 仓库名建议 `driftmaster-legal`（若想用根域名，可命名为 `<你的用户名>.github.io`）
   - 可见性选 **Public**
2. 把本文件夹里的**所有文件和子文件夹**上传到仓库根目录（保持结构：每个子文件夹里是 `index.md`）
3. 仓库 → **Settings → Pages** → Source 选 `Deploy from a branch` → Branch 选 `main` + `/ (root)` → Save
4. 等 1~2 分钟，得到地址：
   - 仓库名是 `<用户名>.github.io` → `https://<用户名>.github.io/privacy-policy/`
   - 仓库名是 `driftmaster-legal` → `https://<用户名>.github.io/driftmaster-legal/privacy-policy/`
5. 逐个打开上面 6 个地址确认都能正常显示（https、公网可访问、无需登录）。

> 用其它托管（Cloudflare Pages / Vercel / Netlify）也可以，但那些平台不会自动把 Markdown 转成网页；需要的话告诉我，我把这 5 份改成自包含 HTML。

## 发布完成后告诉我新域名

我会一次性更新工程里所有引用：

1. **游戏内登录页链接**（4 个）
   - `Assets/Scripts/LoginSceneController.cs`（userAgreementUrl / privacyPolicyUrl / childrenPrivacyUrl / thirdPartyDataUrl）
   - `Assets/Editor/LoginSceneSetup.cs`
   - `Assets/Scenes/LoginScene.unity`（场景里存的值）
2. **法务文档里的交叉链接**
   - `LegalDocuments/Privacy_Policy_CN.md` / `_EN.md` / `_CN_EN.md`
   - `LegalDocuments/Data_Deletion_CN.md` / `_EN.md` / `_CN_EN.md`
   - `LegalDocuments/README.md`
3. **你自己要在 Play Console 更新**
   - 应用内容 → 隐私政策：填新的隐私政策网址
   - 应用内容 → 数据删除：填新的数据删除网址

## 注意

- 网页内容必须与游戏实际行为一致（AdMob 广告、Google Play Games 登录、UGS 云存档、排行榜）
- 儿童隐私与第三方共享清单这两份目前是"游戏内链接指向空值"，发布后建议一并填进登录页
