# vibe-coding-kit

> 给"用 AI 写代码、但自己不太懂技术"的人，一套从想法到上线、还能少走弯路的 Skill 套件。

很多产品经理、创业者、独立开发者现在都在 **Vibe Coding**——把想法甩给 AI，让它写出能跑的东西。但翻车往往不在技术，而在两头：

- **开工前**：需求没说清，AI 朝着错误方向飞速实现。
- **开工后**：AI 越改越乱、功能越加越多、改坏了退不回去、AI 说"做好了"其实没跑通。

这套 Skill 就是来堵这两个口子的。它还有一个更长远的目标：**带一个完全的小白，逐步成长为"能看懂架构、会自己做技术选型"的人。**

## 这套件适合谁

- 不写代码、或刚开始学，靠 AI 把想法变成产品的人。
- 想先跑个 demo 验证想法，又怕跑偏的人。
- demo 验证过了，想认真做成正式系统、但不知从何下手的人。

## 设计理念

- **复杂度是负债** —— 每多一个组件、一个依赖，都是向未来借债。
- **先说问题，再说方案** —— 描述方案会锁死 AI，描述问题才有更优解。
- **不只给答案，更教判断** —— 用得越久，你越不需要照搬话术，因为你已经懂了。
- **知道边界** —— 有些事（动钱、动别人隐私）该找真人，这也是行家的一部分。

## 套件包含 4 个 Skill（按使用时机）

| Skill | 什么时候用 | 里面有什么 |
|-------|-----------|-----------|
| **vibe-coding-requirements** | 想做个 X、跑 demo、跟 AI 对齐需求 | 该不该写代码（阶段零）+ 需求四要素框架 |
| **vibe-coding-architecture** | 选技术栈、看不懂 AI 给的方案 | 看懂架构的 6 维度 + 把 AI 当老师 + 选型五步法 |
| **vibe-coding-production** | demo 想做成正式系统、要部署/上线 | 开发规范 + 安全基线 + 部署 + 验收 + 文档 |
| **vibe-coding-survival** | AI 越改越乱、改坏退不回去、AI 忘事 | 贯穿全程四件事 + 红线 + 项目说明书 |

> **只想跑个 demo？** 你大概只需要 `vibe-coding-requirements`，外加 `vibe-coding-survival` 帮你不翻车。其余两个，等你决定"这东西值得做成正式的"再用。

## 典型路径

```
有个想法
   │
   ├─（先想想要不要写代码）── vibe-coding-requirements ── 把需求说清
   │                                   │
   │                              跑出 demo，验证想法
   │                                   │
   │                          值得做成正式的？
   │                                   │ 是
   │              vibe-coding-architecture ── 看懂架构、选好技术
   │                                   │
   │              vibe-coding-production ── 规范 / 安全 / 部署 / 验收 / 文档
   │                                   │
   └─────── vibe-coding-survival （从第一行代码起，全程配合，避坑 + 自救）
```

## 怎么用 / 安装

每个 Skill 就是 `skills/` 下的一个文件夹，里面有一个 `SKILL.md`——这是通用的 Skill 格式。

```bash
git clone https://github.com/<你的用户名>/vibe-coding-kit.git
```

把需要的 Skill 文件夹接入你的 Claude 即可。**具体接入方式因使用端而异**（Claude.ai 的自定义 Skill、Claude Code 的 Agent Skills、API 等各不相同，且可能更新），请以官方最新文档为准：

- 文档：https://docs.claude.com
- 帮助中心：https://support.claude.com

最简单的用法：你也可以不"安装"，直接把对应那个 `SKILL.md` 的内容复制粘贴进对话，当作给 AI 的指引来用。

## 仓库结构

```
vibe-coding-kit/
├── README.md
├── LICENSE
├── skills/
│   ├── vibe-coding-requirements/SKILL.md
│   ├── vibe-coding-architecture/SKILL.md
│   ├── vibe-coding-production/SKILL.md
│   └── vibe-coding-survival/SKILL.md
└── examples/
    └── 项目说明书-模板.md      ← 复制它，跟着项目一起维护
```

## 一份要随身带的东西

`examples/项目说明书-模板.md` 是把整套流程串起来的活文档。把各个阶段的产出都记进去，每开新对话先贴给 AI——这是对抗"AI 忘事"最有效的一招。

## 贡献

欢迎提 Issue 和 PR：补充话术、修正不准确的地方、增加真实案例。改动 Skill 时请保持"大白话、讲代价、不堆复杂度"的风格。

## License

MIT，见 [LICENSE](./LICENSE)。可自由使用、修改、再分发。
