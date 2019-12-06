# TeXのインストールについて
卒論で使うであろうTeXのインストールなどの説明を書いていきます。
Macは頑張れ
まずTeXはプログラミング言語の一種と考えてもらったほうがいいと思います
だから環境構築が必要ナンデス
## 手順
- 1．installer
これ↓有志の方が作ってくださっているらしいです
https://www.ms.u-tokyo.ac.jp/~abenori/soft/bin/abtexinst_0_91.zip  
- 2 ウィザード起動
ダウンロードした後にそれを解答し実行します  
基本的に「次へ」を押していけば大丈夫です  
参考サイト
http://acetaminophen.hatenablog.com/entry/2015/05/16/142557
インストールに2時間以上かかる場合がデフォです
卒論提出直前にインストール作業を始めるというバカなことをするのはやめよう
~~これまで環境構築さんざんやってきたからわかるよね？~~

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
>\makeatletter  
>\makeatother  

文章の配置の基本設定？加藤さんからもらっていじってないと思う  

>\begin{document}  
>\title{〇〇の△△のための\\××の□\\  
>install}  
>\author{指導教員：aaaaaaa\\  
>bbbb大学 bbbb部\\  
>ccccc学科　dddddd研究室\\  
>ffff年度\\  
>ggggg 永谷園 手馳尾}  
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

表紙の部分終わり  

次は中身についてを書いていこうと思う

## 最後
書き始めはエラーが頻出すると思いますが前年度書いてきた先輩方がいるので頼りましょう
わからなかったら聞いてください
