# Socratic Feynman Tutor

An adaptive tutoring skill for Codex that combines Socratic diagnosis with Feynman reconstruction, transfer testing, and delayed retrieval.

It is designed to optimize for durable, independent ability rather than fluent conversation or short-term recognition.

## What it does

The tutor runs a four-phase learning loop:

1. Map the smallest knowledge gap blocking the learner's goal.
2. Choose the right intervention: Socratic questions, a direct micro-explanation, a worked example, authentic practice, or retrieval practice.
3. Verify understanding through unaided reconstruction, boundary tests, and near or far transfer.
4. Consolidate learning with a retrieval prompt, a transfer task, and a later retention check.

The skill explicitly avoids two common failure modes:

- forcing learners to guess when they are missing a prerequisite;
- declaring mastery from a fluent explanation without independent transfer or delayed retrieval.

## Install

Ask Codex to install the skill from:

```text
https://github.com/wanjeans33/socratic-feynman-tutor
```

Or clone it directly into your Codex skills directory:

```sh
git clone https://github.com/wanjeans33/socratic-feynman-tutor.git ~/.codex/skills/socratic-feynman-tutor
```

Start a new Codex task after installation so the skill can be discovered.

## Use

Invoke it explicitly:

```text
Use $socratic-feynman-tutor to teach me backpropagation.
```

You can also specify an outcome or learning constraint:

```text
Use $socratic-feynman-tutor to help me understand closures well enough to debug JavaScript callbacks. Give direct explanations when I lack a prerequisite, and verify me with a transfer problem.
```

During a session, learner controls include `hint`, `slower`, `harder`, `give me the answer`, `show an example`, `practice mode`, `recap`, and `finish`.

## 中文简介

这是一个面向 Codex 的自适应学习技能。它不会机械地一直追问，而是先诊断学习者的知识边界，再根据问题类型选择苏格拉底提问、直接讲解、示范、真实练习或检索练习。

验证阶段不仅要求学习者用自己的话解释，还会检查概念边界、近迁移、远迁移和独立完成能力。只有经过延迟检索，才会把知识标记为已经保持。

## License

[MIT](LICENSE)
