# Zero-Anxiety Study Skill · 零焦虑五步微课学习模式

> A portable **AI Agent Skill** for turning dense university lectures, English case-based exams, and technical concepts into calm, zero-prerequisite micro-lessons.  
> 一个面向中文学习者与全英文课程备考场景的可复用 **AI Agent 技能（Skill）**，将陌生术语和高压长题干拆解为「每次只推 1 个微知识点 + 1 秒极简练习」的零焦虑学习心流。

---

## 为什么做这个 Skill？/ Why This Skill?

很多同学在用大模型复习全英文专业课（金融科技、AI 伦理、商业数据分析、机器学习等）时，经常遇到三个痛点：
1. **陌生案例壳子焦虑**：英文题干动辄引入一家陌生公司背景，容易误以为“没学过这题”，其实底层只考一个基础公式或概念。
2. **未教先考 & 信息过载**：AI 动不动一口气输出一整屏公式和专业名词，跳过中间分母/前提假设，越看越慌。
3. **听懂了但考场写不出来**：闭卷手写英文简答背不下长难句，或上机断网考试记不清语法易错点。

本 Skill 将经过真实高强度期末复习打磨出的 **「零焦虑五步微课教学协议」** 封装为标准的 `SKILL.md`，支持在 **Antigravity、Codex、Claude Code、Cursor** 等 Agent 工具中即插即用。

---

## 五步标准微课协议 / The 5-Step Micro-Lesson Protocol

1. **剥离外壳（Strip the Shell）**：先用一句话去掉题干里的陌生公司或复杂背景包装，用高中生也能秒懂的大白话讲清底层常识。
2. **中文精讲 + 加粗英文原词（Bold Exam Keywords）**：中文主讲保证零阅读阻力，所有考卷高频词同步强绑定加粗英文原词（如 **out-of-sample $R^2$**、**Deontology**），建立考场条件反射。
3. **极简数字算例 + 干扰项排雷（Worked Example & Trap Alert）**：绝不只丢字母公式，必须代入最简单的整数一步步算清分母和正负号，并直接圈出考官故意放进去的干扰数字。
4. **考场直接变现的高分产物（Exam-Ready Takeaway）**：按考核形式输出「1–3 行手写小抄公式」「三段式 15–25 词短句英文积木模板」或「1 行断网代码肌肉记忆」。
5. **一次一微点 + 1 秒随堂小题（One Micro-Step + 1-Second Quiz）**：严禁未教先考；结尾只留 1 道只需回一个数字/选项/单词的极简题，确认消化后再推进下一个微点。

---

## 快速安装与使用 / Quick Start

### 方式 1：作为 Agent Skill 安装（Codex / Antigravity / Claude Code / Cursor）
将仓库中的 `SKILL.md` 及 `references/` 复制到你的项目或全局 Skills 目录：

```bash
git clone https://github.com/892069773-stack/zero-anxiety-study-skill.git
mkdir -p .agents/skills/zero-anxiety-study-mode
cp -r zero-anxiety-study-skill/SKILL.md zero-anxiety-study-skill/references .agents/skills/zero-anxiety-study-mode/
```

随后在对话中直接说：
> 「开启零焦虑学习模式，带我从零学一遍 Maximum Drawdown（最大回撤）和 Sharpe Ratio。」

### 方式 2：作为 System Prompt 直接使用
直接复制 [SKILL.md](./SKILL.md) 正文到 ChatGPT / Claude / DeepSeek 的自定义指令（Custom Instructions）或项目提示词中即可使用。

---

## 目录结构 / Repository Structure

```text
zero-anxiety-study-skill/
├── SKILL.md                           # 核心技能指令（五步微课教学协议）
├── references/
│   └── pedagogy-checklist.md          # 高中起点可读性与推理连续性检查清单
├── examples/
│   └── sample-micro-lesson.md         # 完整五步微课对话示范（原创合成示例）
├── LICENSE                            # MIT License
└── README.md
```

---

## 致谢与许可 / Acknowledgements & License

- 灵感提炼自香港城市大学 MSc AI in Business 备考期间的 AI 辅助学习实践，并参考了开源课程笔记工作流 [CercaTrovato/cityu-ai-course-notes](https://github.com/CercaTrovato/cityu-ai-course-notes) 对「高中起点可读性」的理念启发；本仓库仅包含原创通用教学协议与合成示例，不含任何课程原始讲义、题库或录音材料。
- Licensed under the [MIT License](./LICENSE).
