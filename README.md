# TeXのインストールについて
卒論で使うであろうTeXのインストールなどの説明を書いていきます。
Macは頑張れ
## 手順
- 1．installer
これ↓基本ウィザードに従ってハイハイ押してくとよいです  
https://sourceforge.net/projects/texworks.mirror/files/latest/download
## 書き方
参考に私のサンプルのコードを貼っておきます

>\documentclass[11pt, a4paper]{jreport}  

ドキュメントのクラス設定、今回はjrepotってやつ  

>\usepackage[driver=dvipdfm]{geometry} 
>\usepackage[dvipdfmx]{graphicx, color}  
>\usepackage{here}  
>\usepackage{slashbox}  
>\usepackage{plext}  
>\usepackage{times, mathptmx}  
>\usepackage{longtable}  
>\usepackage{colortbl}  
>\usepackage{tabularx}  
>\usepackage{enumerate}  
>\usepackage{comment}  
>\usepackage{url}  
>\usepackage{lscape}  
>\usepackage{multirow}  
>%\usepackage{otf}  

ここまでがおそらくjavaだったりのimportの部分  

>\setlength{\voffset}{0.5truecm}  
>\setlength{\headsep}{2truecm}  
>\setlength{\oddsidemargin}{7.0truemm}  
>\setlength{\evensidemargin}{-5.5truemm}  
>\setlength{\topmargin}{-1truecm}  
>\setlength{\footskip}{25truemm}  
>\setlength{\textwidth}{15truecm}  
>\setlength{\textheight}{22truecm}
>\renewcommand{\thefootnote}{\fnsymbol{footnote}}  
>\renewcommand{\bibname}{参考文献}  
>\makeatletter  
>\makeatother  

文章の配置の基本設定？加藤さんからもらっていじってないと思う  

>\begin{document}  
>\title{〇〇の△△のための\\××の□\\  
>Sophistication of Colloquial Writing Check Database for Academic Report Writing}  
>\author{指導教員：aaaaaaa\\  
>bbbb大学 bbbb部\\  
>ccccc学科　dddddd研究室\\  
>ffff年度\\  
>ggggg 長谷川 哲生}  
>\date{\today}  

todayで勝手に印刷のひづけになってくれる  

>\maketitle  
>\pagenumbering{roman}  
>\tableofcontents  
>\input{chapter1.tex}  
>\input{chapter2.tex}  
>\input{chapter3.tex}  
>\input{chapter4.tex}  
>\input{chapter5.tex}  
>\input{chapter6.tex}  
>\input{biblio.tex}  
>\input{thanks.tex}  

上のinput内でtexファイル指定で連続で表示して更にpdfで全部繋がって表示してくれる  

>\end{document}  

終わり  

## 最後

わからなかったら聞いてください
