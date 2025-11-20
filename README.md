# Text2Card: 极简·文读 (v11.0) ✍️➡️🖼️
将长文章秒变小红书卡片 | Markdown to Carousel Generator

“写作是线性的，但阅读可以是卡片式的。”

## 📖 简介 (Introduction)
Text2Card (极简·文读) 是一款专为内容创作者打造的纯前端排版工具。

很多创作者（尤其是从公众号/博客迁移到小红书/Instagram的作者）都面临一个痛点：写好的长文章，需要花费大量时间在 Canva 或 PS 里进行拆分、排版和导出。

本项目通过智能算法，自动将 Markdown 文本流“切割”成适合移动端阅读的 3:4 竖屏卡片。它不仅仅是简单的截断，而是智能识别段落和列表，确保跨页阅读的连贯性。

## ✨ 核心特性 (Key Features)
1. 🧠 智能分页算法 (Smart Pagination Engine)
这是 v11.0 版本的核心黑科技。不同于普通的截图工具，它拥有“语义感知”能力：

防截断保护：不会把一行文字拦腰切断，永远在段落或句子结束处分页。

完美序列 (Perfect Sequence)：当有序列表（Ordered List）跨页时，第二页的序号会自动从上一页结束的地方接续，而不是重置为 "1"，也不会出现突兀的黑点。

标题自适应：首图显示大标题，续页自动生成“标题 / 续”的页眉导航。

## 2. 🎨 三大质感主题 (Aesthetic Themes)
内置三种经过精心调色的阅读模式，适配不同情感的内容：

📜 米白 (Paper)：模拟道林纸纹理，适合人文、历史、小说类内容，自带书卷气。

⚪ 纯白 (White)：极简现代风，适合干货分享、教程、职场类内容。

⚫ 暗黑 (Dark)：沉浸式夜间模式，适合情感、深夜随笔或科技类内容。

## 3. ⚡ 极速工作流 (Lightning Workflow)
Markdown 原生支持：直接粘贴 Markdown 文本，自动渲染 H1, H2, 引用, 列表等样式。

所见即所得：左侧编辑，右侧实时预览。

一键批量导出：基于 html2canvas 技术，一键生成所有分页的高清 PNG 图片（Card_1, Card_2...），直接上传小红书。

## 4. 🔒 隐私安全 (Privacy First)
单文件架构：所有逻辑都在一个 HTML 文件中。

零数据上传：你的文章内容、生成的图片完全在本地浏览器处理，不经过任何服务器。

## 🚀 快速开始 (Quick Start)
下载本项目中的 .html 文件到本地。

双击打开（建议使用 Chrome 或 Edge 浏览器）。

左侧栏设置：

输入 Title（支持 Markdown 语法）。

粘贴文章内容到 Content 区域。

设置 Footer（如：@你的小红书ID）。

选择喜欢的主题颜色。

点击 “立即生成” 查看排版效果。

满意后，点击 “批量下载” 获取图片包。

## 🛠️ 技术细节 (Under the Hood)
本项目采用纯原生技术栈，无构建流程，即开即用：

Core: Vanilla JavaScript (ES6+)

Styling: Tailwind CSS (via CDN)

Markdown Engine: Marked.js

Image Generation: html2canvas

Font: Noto Serif SC (思源宋体) - 营造文学质感

## ⚠️ 注意事项 (Notes)
网络依赖：由于使用了 Tailwind CSS 和 Google Fonts 的 CDN，使用时请保持网络连接。

图片尺寸：默认输出尺寸为 600px * 800px (3:4)，这是小红书笔记的最佳展示比例。

## 🤝 贡献 (Contribution)
如果你有前端开发经验，欢迎在以下方面共创：

增加“封面生成器”（专门用于生成小红书的大标题封面）。

添加更多的字体选择（如手写体）。

优化移动端的编辑体验。
