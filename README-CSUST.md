# 长沙理工大学硕士学位论文 LaTeX 模板

本模板基于 THUThesis（清华大学学位论文 LaTeX 模板）修改，适配长沙理工大学硕士学位论文格式规范。从摘要部分开始，所有格式均已调整为与长沙理工大学论文要求一致。


## 使用方法

### 编译命令

```bash
xelatex thuthesis-example.tex
bibtex thuthesis-example
xelatex thuthesis-example.tex
xelatex thuthesis-example.tex
```

或使用 `latexmk`：

```bash
latexmk -xelatex thuthesis-example.tex
```

### 填写论文内容

在 `thusetup.tex` 中修改论文标题、作者、导师等基本信息。在 `data/abstract.tex` 中填写中英文摘要和关键词。在 `data/chap01.tex` 等文件中编写各章节正文内容。在 `ref/refs.bib` 中添加参考文献条目。在 `data/acknowledgements.tex` 中编写致谢内容。

### 自定义调整

如需微调格式，请修改 `csust-format.sty` 文件中的相应部分，每个格式项目均有清晰的注释说明。

## 注意事项

建议使用 TeX Live 2021 或更新版本编译。编译时需使用 XeLaTeX 引擎。首次编译可能需要下载字体，请确保网络连接正常。如遇字体问题，可在 `thuthesis-example.tex` 的 `\documentclass` 选项中指定 `fontset`（如 `fontset=windows` 或 `fontset=fandol`）。

```bash
长沙理工大学AI Lab出品
```