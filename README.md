# 不背药化 · 官方静态站点

极简静态官网，用于微信开放平台「微信登录」审核 + 应用商店上架所需的官网 / 隐私政策 / 用户协议。

## 文件
- `index.html` 应用介绍页（官网）
- `privacy.html` 隐私政策
- `terms.html` 用户协议
- `style.css` 共享样式

## 上线前需替换的占位
- 隐私政策 / 用户协议中的联系邮箱：`【请替换为你的联系邮箱 …】`
- `index.html` 下载区三个渠道的链接（应用宝 / Google Play / GitHub Releases）
- `index.html` 页脚的 ICP 备案号：`待填写`
- 如需改品牌色，改 `style.css` 顶部 `--accent` / `--accent2`

## 托管

### GitHub Pages（推荐，免费）
1. 新建仓库（如 `btyh-site`），把本目录文件推上去；
2. 仓库 Settings → Pages → Source 选 `main` 分支、`/（root）`；
3. 等待片刻，访问 `https://<用户名>.github.io/<仓库名>/`；
4. 隐私政策 URL 即 `…/privacy.html`，用户协议即 `…/terms.html`。

### Vercel
- 方式 A：把本目录推到 Git 仓库，Vercel 导入该仓库，Framework 选 "Other"，Output 目录留空（根目录）；
- 方式 B：本地直接拖拽本目录到 Vercel Dashboard 的 "Deploy" 区。
- 部署后域名即为官网地址，子页面同上为 `/privacy.html`、`/terms.html`。

## 备注
- 链接均为相对路径（`privacy.html`），GitHub Pages / Vercel 均可直接使用；
- 微信开放平台与应用商店通常要求隐私政策页可公开访问且无需登录，本静态页满足。
