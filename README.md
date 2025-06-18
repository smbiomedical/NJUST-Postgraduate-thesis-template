# NJUST-Thesis-Template

A LaTeX thesis template for Nanjing University of Science & Technology

南京理工大学学位论文Latex模板（硕博）

由于现有的Latex模板年久失修，且不适配Overleaf等在线写作平台。本模板的希望能做到为广大校友提供一个写作方式新选择。
由于作者能力有限，欢迎P/R。本模板会一直保持维护状态。

## 已测试编译环境

1. Overleaf + XeLaTeX ✅
2. Windows + TeX live 2023 + XeLaTeX ✅

## 注意事项

1. 本模板对Overleaf极为友好，编译时需要将compiler设置为XeLaTeX。
2. 如果出现 `Package fontspec Warning: Font "FandolSong-Regular" does not contain requested Script "CJK"`的类似警告，需要手动指定当前操作系统中的CTeX默认字库（如Linux或Overleaf）。例如，在 `njusttt.cls`中设置 `fontset=ubuntu或windows`：
   ```
   \LoadClass[a4paper,zihao=-4,UTF8,fontset=ubuntu]{ctexbook}
   ```

   正常情况下，该警告不影响生成效果，可以直接忽略。
3. 在TeX live环境下，可能会遇到\bibliography报错的情况，需要把编译链中的bibtex换成biber，具体可参考[Issue#1](https://github.com/pasteller/njusttt/issues/2#issue-2511395379)。

## 致谢

本模板修改自前人的成果，包括但不限于：

1. njustThesis：https://github.com/jiec827/njustThesis
