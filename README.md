# Basic English Coach

一个面向中文母语者的英语学习 Skill。它借鉴 C.K. Ogden Basic English 的思路，用更小的核心词汇、短句、间隔复习和即时练习，帮助你把英语变简单、变可记、变得能马上开口使用。

它不是只给答案的翻译器，也不是默认开始讲语法的教材。它更像一个轻量学习教练：先确认你的目标，再带你练习，并在适合的时候先测试、后讲解。

## 安装

```bash
npx skills add haozai007/basic-english-coach
```

或者直接克隆到 Codex skills 目录：

```bash
git clone https://github.com/haozai007/basic-english-coach.git ~/.codex/skills/basic-english-coach
```

如果 Skill 没有立即出现，请重启或重新加载你的 Agent runtime。

## 适合用来做什么

### 1. 背单词

每次学习一组高频词。每个词包含中文释义、简单英语解释、例句、记忆钩子、练习题和下次复习时间。

```text
用 Basic English 帮我学 10 个工作中常用的英语单词。
```

### 2. 间隔复习

按照艾宾浩斯遗忘曲线的思路安排复习。复习时先测试，不提前展示答案；答错的词会在本节课末尾再次出现。

```text
我昨天学了 make, get, take, put, have。请按间隔复习法先考我。
```

### 3. 中文翻译成简单英语

同时输出两个版本：

- `Basic-English-like`：尽量使用短句、常见词和简单结构。
- `Natural simple English`：更自然，更适合现代工作场景。

```text
翻译成简单英语：这个项目我们需要尽快推进，麻烦你看一下有没有什么问题。
```

### 4. 职场英语

围绕具体工作场景生成可以直接使用的表达，例如会议、邮件、客服、软件开发、销售、面试和演示。

```text
我是产品经理，帮我练习需求确认、表达不确定和请求更多信息。
```

### 5. 改写复杂英文

保留原意，把长句拆短，用常见词替换抽象或正式表达，并解释最重要的修改。

```text
把这封英文邮件改得更简单、更清楚。
```

### 6. 复习测验

先测试，再根据错题生成一组更聚焦的小练习。

```text
进入复习模式，先考我 10 题，不要先给答案。
```

## 学习方式

当你提出一个宽泛请求时，Skill 会先确认你的学习目标和英语水平。没有提供水平时，默认按照“中文母语、成人初学者到中低阶、希望学习实用口语和职场英语”来设计练习。

推荐每天练习 15 分钟：

1. 先测试今天到期的词。
2. 只讲解答错或不熟的词。
3. 学习 6 到 10 个新词。
4. 用其中 3 个词造短句。
5. 在课程末尾重测错词。
6. 记录每个词的下次复习时间。

默认复习节奏：

```text
20 分钟后 -> 1 天后 -> 2 天后 -> 4 天后 -> 7 天后 -> 15 天后 -> 30 天后
```

每个词会按照你的回答标记为：

- `Again`：答错、空白或猜测，本节课末尾和第二天再次复习。
- `Hard`：部分答对但不熟，第二天和两天后再次复习。
- `Good`：基本答对，进入下一个正常间隔。
- `Easy`：快速答对，进入更长的间隔。

## 推荐提示词

### 每日学习

```text
请用 Basic English Coach 帮我学习：
目标：提升会议表达
场景：产品需求评审
我的英语水平：初中到高中之间
今天想练：确认需求、表达不确定、请求更多信息
```

### 继续昨天的复习

```text
这是我昨天学过的词：
make | Good | tomorrow | remember: make a change
clear | Again | end of lesson + tomorrow | confused with clean

请先测试我，不要提前展示答案。
```

### 简化英文

```text
把下面这段英文改成简单英语。
请保留原意，拆分长句，并告诉我最重要的修改。
```

## 设计原则

- **先练习，后解释**：需要记忆时，先测试，不提前展示答案。
- **实用优先**：先给可以直接使用的短句，不默认讲长篇语法。
- **简单但不机械**：中文长句会按英语表达习惯重组，而不是逐词翻译。
- **按需加载资料**：不同任务只读取最相关的 reference，减少上下文浪费。
- **不假装纯正**：没有经过词表验证时，使用 `Basic-English-like`，不声称严格符合 Ogden 原始词表。

## Basic-English-like 是什么意思

这个 Skill 受到 C.K. Ogden Basic English 学习哲学的启发，但不尝试复刻完整历史词表。

`Basic-English-like` 表示尽量遵循这种精神：短句、常见词、简单结构。现代职场中，有时仍然需要使用 `requirement`、`feature`、`issue` 等词。这时 Skill 会同时给出更自然的简单职场英语版本。

## 仓库结构

```text
.
├── SKILL.md
├── README.md
├── LICENSE
├── test-prompts.json
├── agents/
│   └── openai.yaml
└── references/
    ├── basic-english-principles.md
    ├── sentence-patterns.md
    ├── translation-style.md
    ├── usage-guide.md
    ├── word-list.md
    └── workplace-scenarios.md
```

## 测试

`test-prompts.json` 包含基础验收场景：

- 职场高频词学习计划
- 中文长句转简单英语
- 先测试、后讲解的间隔复习

## License

MIT
