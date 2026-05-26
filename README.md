# Causal Mechanism Diagram Workflow

因果机制图分析工作流：一个从自然语言到可视化机制图的完整方法论框架。

## 项目背景

在社会科学定性研究中，将文字描述的因果机制转化为可视化图形是一项核心但容易出错的工作。本工作流提供一套结构化的方法——通过五个可重复的方法论步骤（AI辅助执行）+ 一步人工判断（研究者主导），帮助研究者：
1. 将自己的机制推理从自然语言转化为结构化的箭头骨架
2. 系统性地审计每条箭头的因果有效性
3. 生成 Mermaid 初稿代码
4. 审查图形逻辑并接收修改建议
5. 由研究者完成最终的因果判断和人工修改
6. 撰写终稿说明和三个反思段落

## 工作流概览

[➡️ 查看完整工作流](./workflow/00-overview.md)

```
自然语言机制段落
    ↓
Step 1  文字 → 箭头骨架              ← workflow/01-arrow-converter.md
Step 2  因果机制审计                  ← workflow/02-audit.md
Step 3  输出 Mermaid 初稿代码         ← workflow/03-viz-generator.md
Step 4  图形逻辑审查与修改建议        ← workflow/04-graph-audit.md
Step 5  人工修改终稿                  ← 你的因果判断
Step 6  终稿说明 + 三个反思           ← workflow/05-reflection-writer.md
    ↓
可提交的机制图 + 过程记录
```

## 使用方法

1. 准备好你的机制文字段落
2. 从 Step 1 开始，按顺序执行
3. 每一步的 AI 输出都需要你的人工判断
4. Step 5 由你亲手完成——这是最关键的环节
5. 参考 submission/ 下的模板准备提交物

## 目录结构

```
causal-mechanism-diagram-workflow/
├── README.md                  # 本文件
├── workflow/                  # 六步方法论文档
│   ├── 00-overview.md         # 工作流总览
│   ├── 01-arrow-converter.md  # Step 1：文字→箭头
│   ├── 02-audit.md            # Step 2：机制审计
│   ├── 03-viz-generator.md    # Step 3：Mermaid 代码生成
│   ├── 04-graph-audit.md      # Step 4：图形逻辑审查
│   └── 05-reflection-writer.md # Step 6：终稿说明与反思
├── examples/                  # 完整走通案例
│   └── sanctions-case.md      # 经济制裁与威权政权巩固
├── template/                  # 输入模板
│   └── mechanism-input.md     # 机制文字准备模板
└── submission/                # 提交物模板
    ├── process-record.md      # 过程记录框架
    └── submission-guide.md    # 提交物格式指南
```

## 适用场景

- 定性/混合方法研究中的因果机制可视化
- 课程作业：机制图 + AI 协作过程记录
- 论文中的机制图初稿制作与审计
- 方法论教学：因果推理、过程追踪、机制性解释

## 理论依据

本工作流的因果机制概念框架主要基于叶成城（2025）关于因果机制的本体论与认识论区分。三问诊断框架（第三变量/反向因果/稳健性）和缺失分类框架（MCAR/MAR/MNAR）是该方法论的直接应用。

Mermaid 图形语法兼容 Typora、Obsidian 等本地 Markdown 渲染器。

## License

MIT
