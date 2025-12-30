# <img src="./logo.svg" width="34" style="vertical-align: middle;"> LLM Output Converter

[![Online Demo](https://img.shields.io/badge/Online-Demo-green)](https://cjl196.github.io/LLM-Output-Converter/)
[![License](https://img.shields.io/badge/License-MIT-blue)](https://github.com/CJL196/LLM-Output-Converter)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-black)](https://github.com/CJL196/LLM-Output-Converter)


LLM输出文本修复与优化工具，专为处理LLM输出的格式问题而设计。借助正则表达式匹配替换功能，它可以帮助你一键修复 LaTeX 公式、还原 HTML 实体、清理多余格式等。

## ✨ 主要功能

- **Latex 公式修复**
  - 行内公式：将 `\(...\)` 转换为 `$...$`
  - 公式块：将 `\[...\]` 转换为 `$$...$$`，并自动优化换行和缩进
- **HTML 实体还原**
  - 将 `&lt;` 还原为 `<`
  - 将 `&gt;` 还原为 `>`
- **Markdown 格式清理**
  - **删除加粗**：移除 `**text**`，保留纯文本
  - **删除分割线**：移除 `---` 分割线
  - **删除引用**：移除 `[cite_start]...` 等特定引用标记
  - **空白清理**：合并多余空格，删除空行
  - **移除所有标题**：将 `# Title` 转换为 `Title`，支持所有层级
- **标题层级调整**
  - **动态提升**：支持自定义 N (1-5)，一键提升所有标题 N 级
  - **动态降低**：支持自定义 N (1-5)，一键降低所有标题 N 级，并自动处理溢出
- **自定义规则**
  - 支持用户添加自定义正则表达式进行查找替换
  - 规则支持启用/禁用管理
- **全局配置**
  - **保护代码块**：开关控制是否忽略代码块（`...` 和 ```...```）中的内容，防止误修改代码
- **完全本地化**
  - 所有规则数据保存在浏览器本地 (localStorage)
  - 无需服务器交互，安全快速

## 🚀 使用方法

1. 打开 [在线工具](https://github.com/CJL196/LLM-Output-Converter/)
2. 在左侧面板选择需要启用的预设规则
3. (可选) 在 **标题层级工具** 中调整标题级别
4. (可选) 在 **全局设置** 中配置代码保护开关
5. (可选) 添加自定义正则替换规则
6. 将待处理的文本粘贴到输入框
7. 点击 **执行转换** 按钮
8. 从输出框复制处理后的结果

## 🛠️ 项目结构

- `index.html`: 单文件应用，包含所有逻辑和样式
- `logo.svg`: 网站图标资源

## 📄 License

MIT License