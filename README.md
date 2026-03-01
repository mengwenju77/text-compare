# 专业文本比对工具 (Text Compare Tool)

这是一个基于 Web 的专业文本比对工具，能够实时对比两个文本的差异，并提供清晰的高亮显示。

## 功能特点

- **并排视图 (Side-by-side)**：清晰地对比左右两侧文本的差异，行号自动对齐。
- **合并视图 (Unified)**：类似于 Git 的差异视图，在一栏中展示所有修改。
- **即时对比**：输入文本后实时计算并展示结果。
- **精美 UI**：基于 Tailwind CSS 构建，拥有现代化、响应式的用户界面。
- **零依赖运行**：项目采用单文件 HTML 方案，通过 CDN 加载 React、Tailwind 和 jsdiff，无需任何构建步骤即可运行。

## 技术栈

- **React 18**: 用户界面逻辑
- **Tailwind CSS**: 响应式样式
- **jsdiff**: 核心文本比对算法
- **Lucide React**: 矢量图标

## 如何使用

1. 下载或克隆本项目。
2. 在浏览器中直接打开 `index.html` 即可开始使用。

## 部署到 EdgeOne (腾讯云)

本项目已集成腾讯云 EdgeOne Pages 的自动部署流程。

### **方案 A：GitHub Actions 自动部署 (推荐)**

1.  在腾讯云控制台获取 **EdgeOne API Token**。
2.  在 GitHub 仓库的 **Settings > Secrets and variables > Actions** 中添加一个名为 `EDGEONE_API_TOKEN` 的 Secret。
3.  每次向 `main` 分支推送代码时，都会自动触发 GitHub Actions 部署到 EdgeOne。

### **方案 B：EdgeOne Pages 控制台部署**

1.  登录 [腾讯云 EdgeOne 控制台](https://console.cloud.tencent.com/edgeone)。
2.  进入 **站点管理 > Pages**，点击 **创建项目**。
3.  选择 **导入 Git 仓库**，连接你的 GitHub 账号并选择此项目。
4.  配置项目设置：
    -   **构建命令**：(保持为空)
    -   **产物目录**：`.` (或者直接输入 `/`)
5.  点击 **开始部署**。

## 许可证

MIT License
