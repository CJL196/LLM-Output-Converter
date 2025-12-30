# <img src="./logo.svg" width="34" style="vertical-align: middle;"> LLM Output Converter

[在线使用](https://cjl196.github.io/LLM-Output-Converter/) | [GitHub 项目](https://github.com/CJL196/LLM-Output-Converter)

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
- **自定义规则**
  - 支持用户添加自定义正则表达式进行查找替换
  - 规则支持启用/禁用管理
- **完全本地化**
  - 所有规则数据保存在浏览器本地 (localStorage)
  - 无需服务器交互，安全快速

## 🚀 使用方法

1. 打开 [在线工具](https://github.com/CJL196/LLM-Output-Converter/)
2. 在左侧面板选择需要启用的预设规则
3. (可选) 添加自定义正则替换规则
4. 将待处理的文本粘贴到输入框
5. 点击 **执行转换** 按钮
6. 从输出框复制处理后的结果

## 🛠️ 项目结构

- `index.html`: 单文件应用，包含所有逻辑和样式
- `logo.svg`: 网站图标资源

## 📄 License

MIT License