# GitHub Actions 环境变量配置 (更新版)

请在您 Fork 的 Rin 仓库中，通过 `Settings` > `Secrets and variables` > `Actions` 来配置以下内容。

---

## 1. Secrets (机密)

**位置**: 在 `机密` 选项卡下，点击 `新建仓库机密` 按钮。

| Secret 名称 | 说明 | 您的值 |
| :--- | :--- | :--- |
| `CLOUDFLARE_ACCOUNT_ID` | **【请替换】** 您在 Cloudflare 获取的 **账户 ID**。 | `<您的 Cloudflare 账户 ID>` |
| `CLOUDFLARE_API_TOKEN` | **【请替换】** 您创建的 `编辑 Cloudflare Workers` **API 令牌**。 | `<您的 Cloudflare API 令牌>` |

---

## 2. Variables (变量)

**位置**: 先点击 `变量` 选项卡，然后点击 `New repository variable` 按钮。

| Variable 名称 | 说明 | 建议值 (可直接使用) |
| :--- | :--- | :--- |
| `DB_NAME` | 您的 D1 数据库名称。 | `rin-db` |
| `WORKER_NAME` | 您的 Cloudflare Worker 名称。 | `rin-server` |
| `FRONTEND_URL`| **【请替换】** 您部署的前端 Pages 地址。 | `https://<您的-pages-项目名>.pages.dev` |

**S3/R2 相关变量 (暂时无需填写):**

| Variable 名称 | 建议值 (可直接使用) |
| :--- | :--- |
| `S3_BUCKET` | `rin-images` |
| `S3_REGION` | `auto` |
| `S3_ENDPOINT` | (留空) |
| `S3_ACCESS_HOST`| (留空) |
| `S3_FOLDER` | `images/` |
| `S3_CACHE_FOLDER`| `cache/` |

**SEO 相关变量 (可选, 暂时无需填写):**

| Variable 名称 | 建议值 (可直接使用) |
| :--- | :--- |
| `SEO_BASE_URL` | (留空) |
| `SEO_CONTAINS_KEY`| (留空) |