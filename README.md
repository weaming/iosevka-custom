# My custom iosevka

Iosevka 定制构建配置（v34.8.0）：终端、编辑器与网页字体的构建计划及产物。

| 计划 | 用途 | 间距 | 字重 | 倾斜 | 连字 | 字形名称 |
|---|---|---|---|---|---|---|
| `IosevkaTerminal` | 终端 | `term` | Regular、Bold | Upright、Oblique | 启用 | 导出，供 Kitty 使用 |
| `IosevkaCode` | 编辑器与代码 | `normal` | Regular、Bold | Upright、Italic | 禁用 | 导出，供 Kitty 使用 |
| `IosevkaWeb` | 正文网页 | `quasi-proportional` | Regular | Upright | 启用 | 不导出 |
| `IosevkaWebCode` | 网页代码 | `normal` | Regular、Bold | Upright、Italic | 启用 | 不导出 |

所有计划均使用 Normal 宽度（500）、无衬线、点状 `0` 与单层 `a`。它们共享 `private-emoji-exclude.txt`：排除 Unicode Emoji 属性码位以回退系统彩色 emoji，同时保留 `#`、`*` 和数字。

配置值说明：

- `term`：等宽终端间距，收窄箭头和部分几何符号；`normal`：普通等宽；`quasi-proportional`：适合正文的准比例间距。
- Upright：直立；Oblique：倾斜版；Italic：专门设计的斜体版。
- 禁用连字仅保留字符原始形状；导出字形名称可供 Kitty 使用连字，但会增大字体文件。
