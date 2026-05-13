# Super-paper skill

Zotero 论文精读 skill —— 从 Zotero 提取论文，输出 Obsidian 兼容的八段式结构化 Markdown 总结 + Obsidian Canvas 逻辑流画板。

搭建 Obsidian + Zotero + Claude Code 整套工作流

## 功能

四步工作流：

1. **定位** — 在 Zotero 中按关键词/分类/最近添加搜索论文
2. **提取** — 获取元数据、全文、标注，支持多种 PDF 提取器
3. **结构化总结** — 八段式 Markdown 总结（速览 → 背景 → 方法 → 实验 → 结论 → 参考），全中文输出
4. **逻辑流画板** — 自动生成 `.canvas` 文件，在 Obsidian Canvas 中可视化论文逻辑骨架

## 依赖 Skill

安装本 skill 前，请确保已安装以下 skill：

| Skill | 用途 |
|-------|------|
| [zotero-cli-cc](https://github.com/AlaskGulf/zotero-cli-cc) | Zotero 文献检索、PDF 提取 |
| [obsidian-markdown](https://github.com/AlaskGulf/obsidian-markdown) | Obsidian 兼容的 Markdown 写入 |
| [obsidian-bases](https://github.com/AlaskGulf/obsidian-bases) | Dataview 兼容的数据表格式 |
| [json-canvas](https://github.com/AlaskGulf/json-canvas) | Obsidian Canvas 画板生成 |

## 安装

### 方式一：克隆到用户 skills 目录

```bash
git clone https://github.com/AlaskGulf/super-paper.git ~/.claude/skills/Super-paper
```

### 方式二：通过 Marketplace 安装（如已注册）

```bash
claude skills install super-paper
```

## 使用

在 Claude Code 对话中表达读论文意图即可触发：

```
帮我读一下 Zotero 里那篇 Semantic Communication 的论文
```

或明确调用：

```
/super-paper 读最近添加的论文
```

## 输出示例

- `<论文中文译名>.md` — 八段式结构化总结
- `<论文简写>_logic.canvas` — 论文逻辑流画板
- `<论文简写>_arch.canvas`（按需）— 技术架构画板

## License

MIT
