# Transformer 论文中文翻译（Attention Is All You Need）

https://creativecommons.org/licenses/by-nc-sa/4.0/
https://arxiv.org/abs/1706.03762

本项目是深度学习领域里程碑式论文 **《Attention Is All You Need》** 的**中文翻译版**。

论文原文由 Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin 八位作者于 2017 年发布，首次提出了完全基于自注意力机制的 **Transformer** 模型架构。这一架构不仅取代了当时的主流序列模型（RNN、CNN），更成为了当今大语言模型（如 GPT、BERT等）的核心基础。

## 📖 项目简介

- **原文标题**：Attention Is All You Need
- **原文链接**：https://arxiv.org/abs/1706.03762
- **翻译目标**：提供了一份准确、流畅、易于理解的中文译本，帮助中文读者克服语言障碍，深入掌握 Transformer 的核心思想、模型细节与实验设计。
- **翻译原则**：
    - **准确性优先**：忠实于原文含义，确保技术术语翻译准确。
    - **可读性**：在准确的基础上，使中文表达符合中文读者的阅读习惯。
    - **术语统一**：全文保持核心术语（如 Attention, Self-Attention, Layer Normalization 等）翻译的一致性。

## 🎯 快速开始

### 方式一：直接阅读PDF（推荐）
前往 https://github.com/cnolka/transformer-paper-zh/releases 下载最新版本的PDF文档。

### 方式二：在线阅读翻译
- 主翻译文件：`ms.tex`（编译后的PDF在Release中）
- 各章节源码在对应`.tex`文件中

### 方式三：本地编译
如需修改或查看源码，可本地编译：
```bash
git clone https://github.com/your-username/transformer-paper-zh.git
cd transformer-paper-zh
xelatex ms.tex  # 需要LaTeX环境
```

## 📁 项目结构

```
transformer-paper-zh/
├── ms.tex                          # 主文档文件
├── nips_2017.sty                   # 论文样式文件
├── README.md                       # 本文件
├── Figures/                        # 论文图表目录
│   └── ...
├── vis/                            # 可视化相关文件
│   └── ...
└── 各章节源码：
    ├── abstract.tex               # 摘要
    ├── introduction.tex          # 引言
    ├── background.tex            # 背景知识
    ├── model_architecture.tex    # 模型架构（核心章节）
    ├── why_self_attention.tex    # 自注意力机制分析
    ├── training.tex              # 训练细节
    ├── results.tex               # 实验结果
    ├── parameter_attention.tex   # 参数和注意力机制
    ├── sqrt_d_trick.tex          # 缩放点积注意力
    └── visualizations.tex        # 可视化分析
```

## 🛠 编译说明

### 环境要求
- **TeX发行版**：TeX Live 2023+ 或 MiKTeX
- **引擎**：XeLaTeX（支持中文字体）
- **字体**：系统中需安装宋体、黑体等中文字体

### 编译命令
```bash
xelatex ms.tex
bibtex ms.aux
xelatex ms.tex
xelatex ms.tex
```

## ✨ 翻译特色

- **专业准确**：技术术语翻译准确，符合学术规范
- **格式完整**：完全复现原论文的排版风格和章节结构
- **模块化设计**：各章节独立，便于阅读和修改
- **图表完整**：包含原论文所有图表的中文标注版本

## 🤝 参与贡献

欢迎通过以下方式参与改进：

1. **报告问题**：在 https://github.com/cnolka/transformer-paper-zh/issues 中反馈翻译问题或建议
2. **提交修改**：可以 Fork 项目后 Pull Request 提交改进
3. **讨论优化**：对术语翻译或技术表述有更好建议，欢迎讨论

### 贡献指南
- 修改文本内容请编辑对应的`.tex`文件
- 图表相关修改请在`Figures/`目录操作
- 大的结构性改动请先创建Issue讨论

## 📜 许可证

- **翻译内容**：采用 https://creativecommons.org/licenses/by-nc-sa/4.0/ 许可
- **原始论文**：版权归原作者所有
- **样式文件**：`nips_2017.sty` 版权归NeurIPS会议所有

## 🙏 致谢

- 感谢原论文作者的杰出工作
- 感谢LaTeX社区提供的排版支持
- 感谢所有贡献者和审阅者
