# 魔导书 · 原始 Tag 拼接器（magic-prompt）

NovelAI 提示词可视化拼接工具。下拉选项**严格**来自《常规 NovelAI 法典（DOCX）》与《魔导书（XLSX）》原始词库，每个字段均可从词库选择或手动自定义。

## 功能

- 23 类词池（镜头/角度/画风/人物/服装/姿势/场景/质量/负面 …）全部来自原始词库，无自造 fallback tag
- 英文 tag → 中文显示映射（5919 词条，仅影响显示，拼接输出保持英文原 tag）
- 随机抽卡、冲突预检、一键复制
- 可选接入任意 OpenAI 兼容接口（右上角「模型」设置，Key 只存在浏览器 localStorage）

## 部署

纯静态页面，任意静态托管可用：

- 线上地址（GitHub Pages）：https://782042369.github.io/magic-prompt/
- 本地使用：直接用浏览器打开 `index.html`

## 文件

| 文件 | 说明 |
| --- | --- |
| `index.html` | 页面与拼接逻辑 |
| `source-vocabulary.js` | `window.MAGIC_SOURCE` 原始词库（唯一词汇来源） |
| `translations-zh.js` | `window.MAGIC_ZH` 英文 tag → 中文显示映射 |
