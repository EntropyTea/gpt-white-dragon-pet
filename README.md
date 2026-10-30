# GPT白龙娘

银白长发、紫瞳、白色弯角、浅紫龙翼与卷尾的 GPT 龙娘 Pets 素材。

本仓库收录已完成并通过校验的 **Pets v2 精灵图、9 种状态动画和 16 方向视线**。
角色形象及动作设计参考 [bailong-desktop-pet](https://github.com/EntropyTea/bailong-desktop-pet)。

## 动画预览

![完整动画预览](previews/all-states.gif)

[MP4 完整预览](previews/all-states.mp4) · [待机—跳跃—待机](previews/idle-jump-idle.gif) · [视线循环](previews/look-loop.gif)

![关键状态](docs/key-states.png)

## 素材规格

- 精灵图：[assets/spritesheet-v2.png](assets/spritesheet-v2.png)，透明 PNG，1536 × 2288。
- 网格：8 列 × 11 行；单元格 192 × 208。
- 有效帧：73；其余 15 个单元格完全透明。
- [pet.json](pet.json) 记录素材布局、各状态帧数及播放时长。
- 招手与等待回应中包含开合嘴的对话效果；`running` 表示专注思考与处理任务。

| 行 | 状态 | 动作 | 帧数 |
| --- | --- | --- | ---: |
| 0 | `idle` | 待机 | 6 |
| 1 | `running-right` | 向右移动 | 8 |
| 2 | `running-left` | 向左移动 | 8 |
| 3 | `waving` | 招手回应 | 4 |
| 4 | `jumping` | 跳跃 | 5 |
| 5 | `failed` | 失落 | 8 |
| 6 | `waiting` | 等待回应 | 6 |
| 7 | `running` | 思考 | 6 |
| 8 | `review` | 检查结果 | 6 |
| 9–10 | look | 从上方开始顺时针排列的 16 方向视线 | 16 |

每种状态的 GIF 位于 [previews/states](previews/states)。

## 图集与检查

- [全帧联系表](docs/contact-sheet.png)
- [带标签的视线方向表](docs/direction-sheet.png)
- [结构检查](qa/structure.json)、[综合质量检查](qa/quality.json)、[连续性检查](qa/continuity.json)
- [方向语义记录](qa/direction-semantics.json)、[独立方向盲检结果](qa/blind-validation.json)
- [Pets 官方预检](qa/pets-preflight.json)

最终精灵图 SHA-256：

```text
8e660c592261badbccbcaad5a3fbf5481f6fad6f4e7dc64bd713b287fcd2f64f
```

本仓库中的精灵图采用 Pets v2 固定规格；预览文件保留相应的关键帧播放节奏。
