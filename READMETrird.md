[1.インストール](https://github.com/HasegawaTetsuo/TeXinstall/blob/master/README.md)
[2.基本](https://github.com/HasegawaTetsuo/TeXinstall/blob/master/READMESecond.md)

## グラフの置き方
TeXで
```TeX
\begin{figure}[H]
	\centering
	\includegraphics[width=80mm]{./pic/model.png}
	\caption{学習モデルの例}
	\label{model}
\end{figure}
```
パッと書くとこんな感じ
```TeX
\begin{figure}
```
でグラフ置きます宣言  
```TeX
\end{figure}
```
でそこまでにいろいろ設定書きますよって感じ  
```TeX
\centering
```
で表示する際に真ん中に置くことを宣言  
```TeX
\includegraphics[width=80mm]{./pic/model.png}
```
グラフをおきますわよと宣言したのち、後ろの部分で画像のpath指定  
```TeX
\caption{学習モデルの例}
```
グラフの表示名を書いておく  
```TeX
\label{model}
```
TeX内で使うラベル付け、今回は***モデル***  