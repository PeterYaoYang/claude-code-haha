# 01-入门基础

这一组文档是整个学习路线的地基。

如果这些概念还没有理顺，后面看源码会越来越乱。

这组基础课统一按下面这套方式写：

- 先讲概念
- 再讲 Claude Code 在这件事上的实现思路
- 最后再给源码落点

这样读者不会一上来就被文件路径淹没，而是先知道“应该带着什么问题去看代码”。

## 这一组主要解决什么

- model / agent / runtime / tool / command 分别是什么
- 它们是怎么被接成最小 agent 闭环的
- harness engineering 为什么重要
- context / context engineering 是什么
- prompt / instruction design 是什么
- permission / safety boundaries 是什么
- task / workflow / orchestration 是什么

## 建议阅读顺序

1. [01-核心概念与最小闭环.md](./01-核心概念与最小闭环.md)
2. [02-Harness-Engineering.md](./02-Harness-Engineering.md)
3. [03-Context-Engineering.md](./03-Context-Engineering.md)
4. [04-Prompt-Instruction-Design.md](./04-Prompt-Instruction-Design.md)
5. [05-Permission-Safety-Boundaries.md](./05-Permission-Safety-Boundaries.md)
6. [06-Task-Workflow-Orchestration.md](./06-Task-Workflow-Orchestration.md)

## 这一组适合谁

- 我是新手
- 我总在混淆几个核心名词
- 我想先打好概念基础，再去看 Claude Code 源码

## 为什么顺序是这样排的

因为学习顺序最好是：

- 先知道系统由什么组成
- 再知道系统怎么运转
- 再知道为什么同模型同工具效果还会不同
- 再理解 `context` 这种决定模型“看见什么”的层
- 再理解 `prompt` 这种决定模型“该怎么做”的层
- 然后再往里拆 `permission`、`task flow` 这些真正影响行为的层

## 后面这一组还会怎么扩

第一批入门基础现在已经补齐了。

如果后面继续往下补，我会优先补这些更细的基础主题：

- session / state / memory 的进一步拆分
- plan mode 与普通模式的区别
- 多 agent 结果回流与收敛
