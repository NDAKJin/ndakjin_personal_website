# NDAKJin Personal Website

NDAKJin 的个人主页，展示个人项目、ICPC 参赛成绩、兴趣与联系方式。

## 技术栈

- [Astro](https://astro.build/)
- 静态 HTML / CSS

## 环境要求

- Node.js `v24.19.0`
- npm `11.18.0`

## 本地启动

请先安装上述版本的 Node.js，然后执行：

```bash
npm install
npm run dev
```

打开终端显示的本地地址，默认是 `http://localhost:4321`。

## 构建与预览

```bash
npm run build
npm run preview
```

构建产物位于 `dist/`，可直接部署到 Nginx、Caddy 或任意静态文件托管服务。

## 项目结构

```text
src/pages/index.astro  首页内容与样式
public/                静态资源
dist/                  构建产物
```

## 更新服务器

服务器使用 Git 部署时，进入项目目录执行：

```bash
git pull --ff-only
npm ci
npm run build
```

将 Web 服务器根目录指向项目的 `dist/` 目录即可。
