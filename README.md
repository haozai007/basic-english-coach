# Basic English Coach

A Codex skill for learning, practicing, simplifying, and translating English with a C.K. Ogden Basic English-inspired approach.

This skill is designed for Chinese-speaking learners who want practical English through:

- Basic-English-like vocabulary drills
- Ebbinghaus-style spaced repetition
- Chinese-to-simple-English translation
- Workplace phrase packs
- Simple sentence rewriting
- Review quizzes and short active practice

## Install

Clone this repository directly into your Codex skills directory:

```bash
git clone https://github.com/haozai007/basic-english-coach.git ~/.codex/skills/basic-english-coach
```

Restart Codex if the skill does not appear immediately.

## Example Prompts

```text
用 Basic English 帮我学 10 个工作中常用词。
```

```text
用艾宾浩斯记忆法帮我背 10 个 Basic English 单词，并告诉我下次复习时间。
```

```text
把这句话翻译成 Basic English 风格：我想确认一下这个需求是否已经被客户接受。
```

```text
我是咖啡师，帮我总结下工作中最高频的 30 句英语。
```

```text
进入复习模式，先考我 10 题，不要先给答案。
```

## What It Does

### Vocabulary Learning

The skill teaches high-frequency words in small groups, with Chinese meanings, simple English explanations, examples, memory hooks, and active recall questions.

### Ebbinghaus Review

New words are scheduled with a default review rhythm:

```text
20 minutes -> 1 day -> 2 days -> 4 days -> 7 days -> 15 days -> 30 days
```

Review answers can be marked as:

- `Again`
- `Hard`
- `Good`
- `Easy`

### Translation

For Chinese-to-English requests, the skill usually gives:

- `Basic-English-like`
- `Natural simple English`
- Chinese explanation
- Optional practice

### Workplace English

The skill can generate role-based phrase packs for meetings, emails, customer support, software work, sales, interviews, presentations, and other workplace scenes.

## Repository Structure

```text
.
├── SKILL.md
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

## Notes

This project is inspired by C.K. Ogden's Basic English learning philosophy. It is not an official edition of Ogden's book and does not attempt to reproduce the full original text.

The phrase `Basic-English-like` is used intentionally when modern workplace words or approximate simplifications are included.

## License

MIT
