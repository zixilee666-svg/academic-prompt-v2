# academic-prompt-v2

> Academic Hub v3.0 — WorkBuddy Agent 一键部署 Prompt 与完整使用说明书

📌 **在线演示**：https://academic-hub-v3-gefyg50v.edgeone.cool  
🔐 **登录凭据**：`admin` / `123456`

---

## 📂 仓库文件说明

| 文件 | 说明 |
|------|------|
| `DEPLOY_GUIDE.md` | ⭐ **完整部署指南** — 包含 WorkBuddy Agent 可直接复制使用的一键部署 Prompt、使用说明、问题排查、自定义配置 |
| `README.md` | **快速上手** — 核心功能一览、技术栈、本地开发命令 |
| `DEPLOY.md` | **详细部署文档** — EdgeOne Pages 完整配置说明、Cloud Functions + KV 扩展指南 |

---

## 🚀 一键部署（WorkBuddy Agent 使用方法）

### 步骤 1：打开 WorkBuddy Agent

### 步骤 2：复制以下 Prompt 并粘贴到对话窗口

```markdown
## 任务：部署 Academic Hub 学术中心到 EdgeOne Pages

### 项目位置
D:\Users\Lenovo\Desktop\test01-use\input\academic-hub-v3

### 执行步骤

1. cd 到项目目录，安装依赖：
   npm install

2. 构建项目：
   npm run build

3. 部署到 EdgeOne Pages：
   npx edgeone pages deploy -n academic-hub --site-name academic-hub --description "Academic Hub - 学术论文管理与 AI 助手平台" --dist dist

4. 返回部署后的线上 URL
```

### 步骤 3：Agent 将自动完成以下全部流程

```
✅ npm install          → 安装 488 个依赖包
✅ npm run build        → Vite 构建生成 dist/ 产物
✅ edgeone pages deploy → 一键部署到 EdgeOne Pages CDN
✅ 返回线上访问 URL
```

> 💡 **无需手动干预**：整个流程完全自动化，包括依赖安装、项目构建、CDN 部署。

---

## 🛠️ 功能概览

| 路由 | 功能 |
|------|------|
| `/#/` | 📊 仪表盘 — 阅读热力图、统计卡片 |
| `/#/library` | 📚 文献库 — 论文搜索、筛选、引用导出 |
| `/#/my-library` | 📂 文献库管理 — 文件夹增删改、论文分配 |
| `/#/materials` | 📄 个人资料 — PDF/笔记/链接上传、分类管理 |
| `/#/ai-chat` | 💬 AI 对话 — 贞德人格学术助手 |
| `/#/research` | 🔬 我的研究 — 项目与目标追踪 |
| `/#/settings` | ⚙️ 设置 — 深色/浅色模式切换 |

---

## ⚙️ 技术栈

- React 19 + TypeScript 6 + Vite 8
- Tailwind CSS 3.4 + shadcn/ui
- Framer Motion 12（页面过渡动画）
- React Router 7（HashRouter）
- EdgeOne Pages（静态部署）

---

## 📄 许可证

MIT License
