# HTML/Markdown 实时预览工具

一个简洁高效的在线 HTML 和 Markdown 实时预览工具，支持代码编辑和即时渲染。

![HTML/Markdown Preview Tool](https://img.shields.io/badge/HTML-Markdown-blue?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen?style=flat-square)

## ✨ 功能特性

### 🚀 核心功能
- **双模式支持**: 一键切换 HTML 和 Markdown 预览模式
- **实时渲染**: 代码输入即时显示预览效果，无需刷新
- **全屏预览**: 支持全屏模式查看渲染效果，提升预览体验
- **响应式设计**: 完美适配桌面和移动设备

### 💎 技术亮点
- **零配置**: 开箱即用，无需安装任何依赖
- **纯前端**: 基于浏览器技术，数据安全本地处理
- **高性能**: 优化的渲染机制，流畅的用户体验
- **现代 UI**: 基于 Tailwind CSS 的简洁美观界面

### 📝 Markdown 支持
- ✅ 标准 Markdown 语法完整支持
- ✅ 代码块语法高亮
- ✅ 表格渲染
- ✅ 任务列表
- ✅ 引用块
- ✅ GitHub 风格样式

## 🎯 使用场景

- **前端开发**: 快速预览 HTML 代码效果
- **文档编写**: Markdown 文档实时预览和编辑
- **学习工具**: HTML/Markdown 语法学习和练习
- **内容创作**: 博客文章、技术文档编写预览
- **代码演示**: 快速展示代码效果

## 🚀 快速开始

### 在线使用
直接在浏览器中打开 `index.html` 文件即可开始使用。

### 本地部署
```bash
# 克隆项目
git clone https://github.com/lhqs1314/html-and-markdown-preview.git

# 进入项目目录
cd html-preview

# 使用任意 HTTP 服务器启动（可选）
# 方法1：使用 Python
python -m http.server 8000

# 方法2：使用 Node.js
npx serve .

# 方法3：直接双击 index.html 打开
```

访问 `http://localhost:8000` 即可使用。

## 🎮 使用说明

### HTML 模式
1. 点击顶部 "HTML" 按钮切换到 HTML 模式
2. 在左侧编辑器中输入 HTML 代码
3. 右侧实时显示渲染效果
4. 点击 "全屏预览" 查看完整效果

### Markdown 模式
1. 点击顶部 "Markdown" 按钮切换到 Markdown 模式
2. 在左侧编辑器中输入 Markdown 语法
3. 右侧实时显示渲染的 HTML 效果
4. 支持所有标准 Markdown 语法

### 快捷操作
- **切换模式**: 点击顶部 HTML/Markdown 按钮
- **全屏预览**: 点击右上角全屏按钮
- **退出全屏**: 按 ESC 键或点击退出按钮

## 🛠️ 技术架构

### 技术栈
- **前端框架**: 原生 JavaScript (Vanilla JS)
- **样式框架**: Tailwind CSS
- **Markdown 解析**: Marked.js
- **构建工具**: 无需构建，纯静态文件



### 核心特性实现
- **实时预览**: 基于 `input` 事件监听和 `iframe` 动态更新
- **模式切换**: JavaScript 状态管理和 DOM 操作
- **Markdown 渲染**: Marked.js 库解析 + 自定义 CSS 样式
- **全屏功能**: CSS Modal + JavaScript 事件处理

## 🌟 特色功能详解

### 双模式预览
- **HTML 模式**: 直接渲染 HTML 代码，支持内联 CSS 和 JavaScript
- **Markdown 模式**: 将 Markdown 转换为带样式的 HTML 页面

### 实时同步
- 输入内容变化时立即更新预览
- 全屏模式与主预览保持同步
- 模式切换时智能加载示例内容

### 用户体验优化
- 平滑的过渡动画效果
- 响应式布局适配
- 键盘快捷键支持
- 无黑屏闪烁的全屏切换

## 🎨 自定义配置

### 修改 Markdown 样式
编辑 `getMarkdownHtmlTemplate` 函数中的 CSS 样式：

```javascript
// 自定义 Markdown 样式
function getMarkdownHtmlTemplate(markdownHtml) {
    return `<!DOCTYPE html>
    <html>
    <head>
        <style>
            /* 在这里添加自定义样式 */
            body { 
                font-family: 'Your Font', sans-serif;
                /* 更多样式... */
            }
        </style>
    </head>
    <body>${markdownHtml}</body>
    </html>`;
}
```

### 添加新功能
项目采用模块化设计，易于扩展：
- 添加新的渲染模式
- 集成语法高亮
- 添加导出功能
- 集成云端保存

## 🤝 贡献指南

欢迎提交 Pull Request 和 Issue！

### 开发环境设置
1. Fork 本仓库
2. 创建特性分支: `git checkout -b feature/your-feature`
3. 提交更改: `git commit -am 'Add some feature'`
4. 推送分支: `git push origin feature/your-feature`
5. 提交 Pull Request

### 代码规范
- 使用 ES6+ 语法
- 遵循现有代码风格
- 添加适当的注释
- 确保功能完整测试

## 📄 许可证

本项目基于 [MIT 许可证](LICENSE) 开源。

## 🙏 致谢

- [Tailwind CSS](https://tailwindcss.com/) - 现代化 CSS 框架
- [Marked.js](https://marked.js.org/) - 高性能 Markdown 解析器
- [GitHub](https://github.com/) - 代码托管平台

## 📞 联系方式

- 项目主页: [GitHub Repository](https://github.com/lhqs1314/html-and-markdown-preview)
- 问题反馈: [GitHub Issues](https://github.com/lhqs1314/html-and-markdown-preview/issues)
- 功能建议: [GitHub Discussions](https://github.com/lhqs1314/html-and-markdown-preview/discussions)

---

⭐ 如果这个项目对你有帮助，请给它一个星标！

![GitHub stars](https://img.shields.io/github/stars/lhqs1314/html-and-markdown-preview?style=social)
![GitHub forks](https://img.shields.io/github/forks/lhqs1314/html-and-markdown-preview?style=social)