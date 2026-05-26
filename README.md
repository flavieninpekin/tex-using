# 湖南高考备考资料

为湖南省高考（新课标Ⅰ卷）语数外物化生准备的答题模板和应记应背的公式定理。

## 目录结构

```
├── main.tex                 # 主文档（汇总所有科目）
├── 数学/  ├── 数学.tex                # 独立编译
│          ├── formulas.tex            # 常用公式、定理与结论
│          ├── timing-and-tips.tex     # 答题时间规划与技巧
│          ├── frequency-analysis.tex  # 高考考频分析
│          ├── guided-practice.tex     # 真题代练
│          └── categorized-training.tex  # 分类训练与限时训练
├── 语文/  └── 语文.tex       # 待完善
├── 英语/  └── 英语.tex       # 待完善
├── 物理/  └── 物理.tex       # 待完善
├── 化学/  └── 化学.tex       # 待完善
├── 生物/  └── 生物.tex       # 待完善
└── .github/workflows/
    └── compile-latex.yml     # CI: 推送时自动编译 PDF
```

## 编译方式

**本地**（需安装 TeX Live + XeLaTeX）：
```bash
latexmk -xelatex main.tex          # 全部科目
latexmk -xelatex 数学/数学.tex      # 单科
```

**CI**：推送到 `main` 分支后，GitHub Actions 自动编译并生成 PDF 工件（Artifacts），可在 Actions 页面下载。

## 进度

- [x] 数学 -- 公式定理 + 时间规划与技巧 + 考频分析 + 真题代练 + 分类训练与限时训练
- [ ] 语文
- [ ] 英语
- [ ] 物理
- [ ] 化学
- [ ] 生物
