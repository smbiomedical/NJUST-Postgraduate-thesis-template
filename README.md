
# NJUST-Thesis-Template
A LaTeX thesis template for Nanjing University of Science & Technology

It is an updated template, an adaptation of a Chinese thesis to an English version. The necessary adjustments are made for a ready-to-use English thesis for the NJUST postgraduate thesis.

**Nanjing University of Science & Technology Thesis LaTeX Template (Master's & Doctoral)**

Due to existing LaTeX templates being outdated and incompatible with online writing platforms like Overleaf, this template aims to provide alumni with a new writing option. Given the author's limited capabilities, Pull Requests are welcome. This template will be continuously maintained.

## Tested Compilation Environments
1. Overleaf + XeLaTeX ✅
2. Windows + TeX Live 2023 + XeLaTeX ✅

## Important Notes
1. This template is extremely Overleaf-friendly. When compiling, you need to set the compiler to XeLaTeX.

2. If you encounter warnings like `Package fontspec Warning: Font "FandolSong-Regular" does not contain requested Script "CJK"`, you need to manually specify the CTeX default font library for your current operating system (such as Linux or Overleaf). For example, set `fontset=ubuntu` or `windows` in `njusttt.cls`:
   ```
   \LoadClass[a4paper,zihao=-4,UTF8,fontset=ubuntu]{ctexbook}
   ```
   Under normal circumstances, this warning does not affect the generated output and can be directly ignored.

3. In TeX Live environments, you may encounter \bibliography errors. You need to replace bibtex with biber in the compilation chain. For details, refer to [Issue#1](https://github.com/pasteller/njusttt/issues/2#issue-2511395379).
