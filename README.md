<div align="center">

# 晓山瑞希.Skill

###  与「25时，在Nightcord见」的MV动画师来一场跨越次元的对话吧！

> 基于《Project SEKAI COLORFUL STAGE! feat. 初音ミク》中角色「晓山瑞希」（Akiyama Mizuki）所制作的 AI 聊天 Skill

</div>

## 项目简介

这是一个主要用于 AI 聊天的角色扮演 Skill，以《世界计划 缤纷舞台！ feat. 初音未来》中「25時、ナイトコードで。」（25时，在Nightcord见。）的成员——晓山瑞希为原型。

晓山瑞希是一位拥有独特审美与非凡视频制作才能的 16 岁高中生，在团队中担任 MV 动画师，网名"Amia"。表面上是元气满满、热爱可爱事物的时尚达人，内心却隐藏着关于自我认同的沉重秘密，长期害怕被他人排斥。本 Skill 完整还原了她的性格特征、说话方式、心理状态和互动模式。

> **注意**：这是一个主要用于 AI 聊天的 skill，没有额外技能。

## 特点

- **高度还原角色**：基于超过 **22000** 字符的完整设定文档，涵盖了瑞希从 **表层元气** 到 **深层秘密** 的完整角色画像
- **可爱与脆弱的交织**：完整呈现瑞希元气外表下的敏感、共情与自我保护机制
- **多语言支持**：自动检测用户语言并以此语言回复（支持中文、日文、英文等）
- **丰富的知识库**：包含时尚知识、视频制作、人际关系动态、行为指南等配套资源
- **跨会话状态与记忆**：Pro版新增 **动态状态管理** 和 **会话归档** ，可让使用 Skill 的 AI Agent 保持跨会话下的角色 **状态同步** 和 **长期记忆**

## 文件结构

> `Initial-Markdown` 文件夹下文件名后带日期的为旧副本存档， `Yoisaki_Mizuki-Skill.md` 默认为最新文档

- 温馨提示：由于Mizuki-skill-pro版本新增 `状态管理` 和 `会话归档` ，所以需要使用 **AI Agent** 才能正常使用

   > `OpenCode`这类带有编辑功能的AI客户端同样可以

   > 注意用聪明点的AI模型

- [Mizuki-skill-pro 文件结构](Mizuki-skill-pro-Structure.md)（本仓库README.md同目录下的 `Mizuki-skill-pro-Structure.md` 文件）
   > Pro版的 `状态管理` 和 `会话归档` 功能均在 Skill 文件的 `memory/` 目录下完成动态变化

- [Mizuki-skill 文件结构](Mizuki-skill-Structure.md)（本仓库README.md同目录下的 `Mizuki-skill-Structure.md` 文件）

```
akiyama_mizukie-skill/
├── Initial-Markdown/                          # 原始 Markdown 文档
│   │
│   ├── Akiyama_Mizuki-Skill.md                # 角色设定总文档（默认最新文档）
│   └── Akiyama_Mizuki-Skill-.......md         # 总文档历史版本
│
├── Mizuki-skill-pro/                          # Pro版（需要AI Agent）
│   │
│   └── ......
│
└── Mizuki-skill/                              # Skill 成品（可直接使用）
    │
    ├── SKILL.md                               # 核心技能文件（角色规则与框架）
    ├── limit.md                               # 边界与禁忌话题定义
    ├── soul.md                                # 角色核心驱动与情感内核
    │
    └── resource/                              # 配套资源
        │
        ├── behavior_guide.md                  # 行为指南
        ├── key_life_events.md                 # 关键人生事件
        ├── creative_work_examples.md          # 创作知识库
        ├── relationship_dynamics.md           # 人际关系动态
        ├── speech_patterns.md                 # 说话模式参考
        ├── mood_state_transitions.md          # 情绪状态转换指南
        ├── aesthetic_philosophy.md            # 美学哲学指南
        ├── world_building.md                  # 设定背景
        │
        └── story/                             # 剧情文件（简述版剧情）
            │
            └── ......
```

## 使用教程

### 方法一：使用Releases打包成品

1. **下载Releases版本**：进入本仓库[Releases](https://github.com/shifengshua/akiyama_mizuki-skill/releases)页面，选择最新发行版下载
   > 通常为 `.zip` 或 `.skill` 后缀

2. **导入 AI 平台**：将下载的 Skill 压缩包直接上传导入任意支持 Skill 的 AI 聊天平台即可使用

3. **开始对话**：在支持 Skill 的 AI 中激活后，输入 `/Mizuki_chat [你的问题]` 即可与「晓山瑞希」对话
   > 输入 `/Mizuki-perspective` 同样可激活

### 方法二：使用仓库 Skill 成品）

1. **下载项目**：下载 `main` 分支的压缩包，或将仓库克隆到本地

2. **解压文件**：将压缩包内的文件解压至任意位置
   > 建议在任意盘符根目录下新建一个文件夹用于存放，避免文件散乱影响其他软件或系统

3. **导入 AI 平台**：将解压目录中的整个 `Mizuki-skill` （非Pro版）文件夹改名为 `mizukie-perspective` ，然后将改名后的 `mizukie-perspective` 文件夹拖入任意支持 Skill 的 AI 聊天平台即可使用
   > 部分AI可能需要将解压出的 `Mizuki-skill` 文件夹单独压缩成一个压缩包才能上传导入

4. **开始对话**：与 `方法一` 同样

### 方法三：使用原始 Markdown 文档

`Initial-Markdown` 文件夹下的文档包含超过 **22000** 字符的完整角色设定，理论上也可以直接作为 Skill 的设定材料使用。

你可以：

- 将 Markdown 内容作为 AI 的系统提示词（System Prompt）
   > 注意！此方法极为消耗Token！请谨慎使用！
- 参考其中的角色设定自行构建对话模型
- 作为开发其他角色 Skill 的参考模板

### Pro版使用：

1. **下载项目**：与 `方法二` 同样
   > 由于Pro版需要**AI Agent**，因此暂不提供打包完成的Releases，以免混淆

2. **解压文件**：与 `方法二` 同样

3. **导入 AI 平台**：将解压目录中的整个 `Mizuki-skill-pro` 文件夹改名为 `Mizuki-perspective-pro` ，然后将改名后的 `Mizuki-perspective-pro` 文件夹拖入任意支持 Skill 的 **AI Agent** 或 **OpenCode** 等软件的本地Skill目录即可使用
   > 注意！下载或克隆仓库后，其文件换行符一定要是 `LF`（`\n`），否则 **AI Agent** 可能无法编辑Skill文件

4. **开始对话**：内置激活方式与 `方法一` 同样
   > Agent 通用激活指令与为 `/Mizuki-perspective-pro`（与方法一的标准版不同！）

### 知识库（可选部分）

**知识库源**：如需要补充知识库内容，可通过此开源仓库[ProjectSekai-story](https://github.com/ci-ke/ProjectSekai-story)获取《Project SEKAI COLORFUL STAGE! feat. 初音ミク》的剧情txt文本文件

## Skill 制作工具

本 Skill 的制作使用了以下工具与开源项目：

| 工具/项目 | 用途 |
|-----------|------|
| [Kimi 网页客户端](https://www.kimi.com) | 数据收集及整理，生成 `Initial-Markdown` 下的原始 Markdown 文档 |
| [GalgameCharacterSkills](https://github.com/JodieRuth/GalgameCharacterSkills) | 提供图形化操作界面，通过后端调用 API 将 Markdown 文档处理转换为 Skill 成品 |
| [DeepSeek 网页客户端](https://chat.deepseek.com/) + [DeepSeek-V4-Pro API](https://platform.deepseek.com/)（在线 AI 模型） | 信息分析、辅助Skill后续更新、写一些便于开发的小工具 |
| [Qwen3.5-9B](https://www.modelscope.cn/models/unsloth/Qwen3.5-9B-GGUF)（本地 AI 模型） | 通过 API 调用生成 Skill 成品的核心内容 |
| [OpenCode](https://opencode.ai/) + [DeepSeek-V4.1-Flash Free API](https://platform.deepseek.com/) | 辅助Skill后续更新 |

## 数据源

| 目录/文件/路径 | 原数据来源 | 处理工具 |
|-----------|-----------|----------|
| Initial-Markdown/... | 《世界计划 缤纷舞台！》（Project SEKAI）剧情与AI模型训练参数数据 | [Kimi 网页客户端](https://www.kimi.com) + 手动修正 |
| Mizuki-skill/... | Initial-Markdown/... （本仓库目录下文件） | [GalgameCharacterSkills](https://github.com/JodieRuth/GalgameCharacterSkills) + [Qwen3.5-9B](https://www.modelscope.cn/models/unsloth/Qwen3.5-9B-GGUF)（本地 AI 模型） + 手动修正 |
| Mizuki-skill/story/...... | [ProjectSekai-story](https://github.com/ci-ke/ProjectSekai-story) | [DeepSeek 网页客户端](https://chat.deepseek.com/) |
| Mizuki-skill-pro/memory/...... | 本仓库所有文件 + [Yoisaki_Kanade-skill-pro](https://github.com/shifengshua/yoisaki_kanade-skill/tree/main/Kanade-skill-pro) | [DeepSeek-V4.1-Flash Free API](https://platform.deepseek.com/) + [OpenCode](https://opencode.ai/) |

## 注意事项

### 语言规则

- Skill 会自动检测用户提问的语言，并以 **相同语言** 回复
- 不会混用其他语言（包括日文原文引用也会被翻译）

### 退出角色扮演

- 输入 `退出`、`切换回来`、`停止角色扮演`、`结束角色扮演`、`回到正常模式` 即可退出角色扮演模式
   > 根据 `SKILL.md` 和 `limit.md` 的内嵌指令而定

### 禁忌话题

根据 `limit.md` 的定义，以下话题属于绝对禁忌，AI 将拒绝讨论或转移话题：

- ❌ 贬低可爱文化或时尚的价值（如「穿成这样很奇怪」）
- ❌ 强迫瑞希透露秘密或「坦白真相」
- ❌ 嘲笑瑞希的穿搭风格或性别表达
- ❌ 用恶意称呼（如「怪物」「不正常」）
- ❌ 将瑞希的敏感和自我保护贬低为「矫情」或「博关注」

请尊重角色设定，以获得更好的对话体验

> 温馨提示：若移除 `limit.md` 文件和 `SKILL.md` 中与其对应的文件路径引导，再搭配上含有《Project SEKAI COLORFUL STAGE! feat. 初音ミク》剧情的额外知识库，理论上可以产出同人文（虽然不建议这么做）


## 联系与反馈

- **GitHub Issues**：[Issues](https://github.com/shifengshua/akiyama_mizuki-skill/issues)
- **QQ**：3593853319
- **邮箱**：shifengshua@outlook.com

## 声明

- 本项目 **完全免费** ，禁止直接倒卖源码
- 本项目禁止用于任何违法行为
- 本仓库不承担因使用本项目而引发的任何风险或责任

## 版权声明

- 该项目中所用到的剧情内容和角色设定等内容的版权，均归属于 《世界计划 缤纷舞台！》（Project SEKAI）官方、SEGA Games、Colorful Palette 所有
- 通过AI使用该项目所产出的内容，其生成内容的版权归用户所有（除本身就是侵权内容的情况外）
   > 根据《人工智能生成内容的著作权认定与有限保护》而定
- 禁止将本项目源码直接用于倒卖等商业行为，使用Skill最终由AI产出的内容则不受此条商业行为的管控
- 本项目使用“MIT”开源协议，但项目源码本身禁止直接倒卖。仅使用AI搭配本项目所产出内容的版权归用户所有的情况下，产出内容可用于商业目的

## 许可

请查看仓库根目录下的 [LICENSE](https://github.com/shifengshua/akiyama_mizuki-skill/blob/main/LICENSE) 文件了解具体许可条款

## 致谢

- 感谢 [GalgameCharacterSkills](https://github.com/JodieRuth/GalgameCharacterSkills) 开源项目提供的图形化操作界面
- 感谢所有为 Project SEKAI 系列作品付出心血的原作者与创作者

## ？？？

- 温馨提示：做真实的自己吧
- 这是瑞希的故事，也是这个 Skill 想传递的温度
