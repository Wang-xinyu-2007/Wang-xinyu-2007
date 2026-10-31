<div align="center">

# Xinyu Wang

**数学系大二 · 从公式到代码实现机器学习**

`Mathematics undergraduate` · `building ML from first principles` · `seeking a 2026–27 winter AI/ML internship`

[![Open to AI/ML internships](https://img.shields.io/badge/Open%20to-AI%2FML%20Internships-2ea44f?style=flat-square)](https://github.com/Wang-xinyu-2007)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)

</div>

---

## 现在

数学系大二，正在把机器学习从“会调用 API”推进到“能推导、能实现、能评测、能解释”。

- 主线：线性代数 / 概率 / 优化 → 手写 ML 基础 → PyTorch 训练与 Transformer
- 目标：**2026–27 寒假 AI/ML 实习**（模型训练与评测、数据管道、研究助理方向都愿意做）
- 方法：每个核心项目都要有可运行命令、测试、held-out 结果和明确的局限

## 精选项目

### [tiny-char-transformer](https://github.com/Wang-xinyu-2007/tiny-char-transformer)

从零实现的 GPT 风格字符级 Transformer：显式因果多头注意力、Pre-LN 残差块、weight tying、AdamW + cosine schedule、自回归采样。

- 818K 参数，4 层 / 4 头 / 128 维，在 Tiny Shakespeare 上 CPU 训练 3,000 步（约 16 分钟）
- 最佳验证损失 **1.8988**（困惑度 **6.68**，随机基线为 65）；1,200 步基线为 2.2156
- 11 个单元测试，包括“未来 token 不能影响前缀 logits”的因果泄漏测试
- 数学推导：[`docs/math.md`](https://github.com/Wang-xinyu-2007/tiny-char-transformer/blob/main/docs/math.md)
- 训练曲线与样本在仓库的 `results/` 下

<img src="https://raw.githubusercontent.com/Wang-xinyu-2007/tiny-char-transformer/main/results/loss_curve.png" width="620" alt="Tiny Char Transformer 训练与验证损失曲线">

### [linreg-lab](https://github.com/Wang-xinyu-2007/linreg-lab)

用 NumPy 从零手写线性回归的五关练习：向量化预测、损失与梯度、正规方程、梯度下降、标准化与 R²。每关都有测试验收。

### 工程基本功

几个零依赖 CLI 工具，用来练边界情况、API 设计和 README 写作，全部有测试和 GitHub Actions：

[`hexpeek`](https://github.com/Wang-xinyu-2007/hexpeek)（C11 hexdump） ·
[`locstat`](https://github.com/Wang-xinyu-2007/locstat)（代码行数统计） ·
[`csvpeek`](https://github.com/Wang-xinyu-2007/csvpeek)（CSV 体检） ·
[`grade-report`](https://github.com/Wang-xinyu-2007/grade-report)（成绩统计报告）

## 技术栈

```text
Language     Python · C
ML           PyTorch · NumPy · Transformer / 注意力机制
Data         pandas · SQL / SQLite
Engineering  pytest · Git · GitHub Actions · CLI 设计
Learning     BPE / tokenizer · KV cache · 优化与概率
```

## 正在做

- [x] 用一个小 Transformer 跑通“推导 → 实现 → 训练 → 评测 → 采样”
- [ ] 给 `changchun-housing` 换真实公开数据，补上结论、baseline 与误差分析
- [ ] 给 Transformer 加 BPE tokenizer / KV cache，并做位置编码与深度 ablation
- [ ] 参与一个开源 ML 项目（从测试、文档或小 bug 开始）

> 我相信作品比标签更有说服力：一个小而完整、能被追问的项目，胜过十个教程复刻。

## 联系

开放 2026–27 寒假 AI/ML 实习。邮箱见个人资料页；也欢迎在任意仓库开 issue 讨论。
