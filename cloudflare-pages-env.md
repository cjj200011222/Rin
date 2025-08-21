# Cloudflare Pages 环境变量

将以下变量和值复制到 Cloudflare Pages 项目的环境变量设置中。

## 构建设置

*   **框架预设**: `无`
*   **构建命令**: `bun b`
*   **构建输出目录**: `client/dist`
*   **根目录**: (留空)

## 环境变量

```ini
NAME=Rin User
DESCRIPTION=A new Rin blog
AVATAR=https://avatars.githubusercontent.com/u/36541432
API_URL=https://temp-rin-api.example.com
PAGE_SIZE=5
SKIP_DEPENDENCY_INSTALL=true
UNSTABLE_PRE_BUILD=asdf install bun latest && asdf global bun latest && bun i
```

**注意:**
- `API_URL` 是一个临时地址，在后端部署完成后需要回来修改成真实的后端地址。
- `SKIP_DEPENDENCY_INSTALL` 和 `UNSTABLE_PRE_BUILD` 是 Cloudflare 用于配置 Bun 构建环境的，请勿修改。