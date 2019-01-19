# HZNUMCM latex类
美赛论文模版

## 1. 使用方法
- Windows环境下安装CTEX，Mac环境下安装macTex，考虑windows环境较多用，以下用CTex为例，主要的编辑器使用winEdt
- 一般新建一个文件夹，将HZNUMCM.cls文件放到当前文件夹中
- 在此文件夹中建一个image为名的文件夹，以后里面将放图片文件
- 新建一个.tex文本文件，自己取好文件名，假设为myfile
- 新建一个.bib文本文件，尽可能与.tex文件同名同文件夹
- 写文件 myfile.tex,代码内容
`\documentclass{HZNUMCM}
`  \setControlNumber{888888}
`  \setContestType{MCM}
`  \setProblemLetter{A}
`  \setPaperTitle{ Title title}
`  \setSummary{ sumary sumary sumary sumary sumary sumary sumary sumary sumary sumary sumary}
`\begin{document}
`  \showSummarySheet
`  \showContents
`\section{aaaaaaa}
`\section{bbbbbbb}
`  \addcontentsline{toc}{section}{References}
`  \bibliographystyle{unsrt}%{brief}%{alpha}%{unsrt}
`  \bibliography{paper}
`\end{document}
 

- myfile.bib文件采用bibtex格式
  
## 2. 使用步骤
- 编辑好内容
- 使用xelatex多编译几次（大于等于二次）、使用bibtex编译几次（大于等于一次），使用xelatex多编译几次（大于等于二次），循环多次直到没有错误
