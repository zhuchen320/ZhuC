# Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

Learn more about IDE Support for Vue in the [Vue Docs Scaling up Guide](https://vuejs.org/guide/scaling-up/tooling.html#ide-support).

## 部署指南

### 方法一：GitHub Pages（推荐）

你的项目已经配置了 `base: '/ZhuC/'`，适合部署到 GitHub Pages。

#### 步骤：

1. **构建项目**
   ```bash
   pnpm build
   ```

2. **安装 GitHub Pages 部署工具（可选）**
   ```bash
   pnpm add -D gh-pages
   ```

3. **在 package.json 中添加部署脚本**
   ```json
   "scripts": {
     "deploy": "pnpm build && gh-pages -d dist"
   }
   ```

4. **部署**
   ```bash
   pnpm deploy
   ```

5. **在 GitHub 仓库设置中启用 Pages**
   - 进入仓库的 Settings → Pages
   - Source 选择 `gh-pages` 分支
   - 保存后访问：`https://你的用户名.github.io/ZhuC/`

### 方法二：Vercel（最简单）

1. **安装 Vercel CLI**
   ```bash
   npm i -g vercel
   ```

2. **部署**
   ```bash
   vercel
   ```
   或者直接访问 [vercel.com](https://vercel.com)，连接 GitHub 仓库自动部署。

**注意**：如果使用 Vercel，需要修改 `vite.config.js` 中的 `base` 为 `/`：
```js
base: '/',
```

### 方法三：Netlify

1. **安装 Netlify CLI**
   ```bash
   npm i -g netlify-cli
   ```

2. **构建并部署**
   ```bash
   pnpm build
   netlify deploy --prod --dir=dist
   ```

或者访问 [netlify.com](https://netlify.com)，拖拽 `dist` 文件夹到网站即可。

**注意**：如果使用 Netlify，也需要修改 `base` 为 `/`。

### 方法四：其他静态托管服务

- **Cloudflare Pages**：连接 GitHub 仓库自动部署
- **Firebase Hosting**：使用 Firebase CLI 部署
- **阿里云 OSS / 腾讯云 COS**：上传 `dist` 目录内容到存储桶并开启静态网站托管

### 部署前检查清单

- [ ] 运行 `pnpm build` 确保构建成功
- [ ] 检查 `dist` 目录是否包含所有文件
- [ ] 根据部署平台调整 `vite.config.js` 中的 `base` 配置
- [ ] 测试生产环境预览：`pnpm preview`
