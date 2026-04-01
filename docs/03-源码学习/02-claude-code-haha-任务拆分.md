# claude-code-haha 任务拆分

## 为什么要先拆分

这个仓库不适合一上来从头到尾硬读。

更好的方式是先拆成几个学习任务，每次只解决一个问题。

## 推荐拆分方式

### 1. 启动链路

重点文件：

- `src/entrypoints/cli.tsx`
- `src/main.tsx`

重点问题：

- Claude Code 怎么启动
- fast path 是什么
- runtime 是怎么装配起来的

### 2. command 系统

重点文件：

- `src/commands.ts`
- `src/commands/`

重点问题：

- command 为什么存在
- command 和 tool 有什么区别
- 用户入口是怎么组织的

### 3. tool 系统

重点文件：

- `src/tools.ts`
- `src/tools/`

重点问题：

- tool 是怎么注册的
- 模型能用哪些能力
- tool description 为什么重要

### 4. permission system

重点文件：

- `src/constants/tools.ts`
- `src/utils/permissions/`

重点问题：

- 为什么 agent 一定要有权限边界
- 主 agent 和子 agent 的能力为什么不同

### 5. task / coordinator / 多 agent

重点目录：

- `src/tasks/`
- `src/coordinator/`
- `src/tools/AgentTool/`

重点问题：

- 多 agent 为什么难
- task 和 message 为什么是基础设施
- coordinator 解决什么问题

### 6. 扩展系统

重点目录：

- `src/services/`
- `src/plugins/`
- `src/skills/`

重点问题：

- Claude Code 如何扩展能力
- services、plugins、skills 分别承担什么职责

## 推荐学习节奏

建议一次只学一个主题：

1. 先学概念
2. 再看对应源码
3. 再写一段自己的理解

不要一次同时啃多个模块。

## 每个主题学完后应该沉淀什么

建议至少记录：

- 这个模块解决什么问题
- 它在整套系统里的位置
- 它和 model / agent / runtime / tool 的关系
- 一两个最关键的源码文件
- 自己原来哪里理解错了
