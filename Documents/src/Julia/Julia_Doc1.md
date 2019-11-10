# Julia 備忘録

* Jupyter Notebook開くコマンド  
```
julia> using IJulia  
julia> notebook()  
```

- ライブラリを入れる手順  
```Julia
(v1.0) pkg> add PyPot  
(v1.0) pkg> add GR  
(v1.0) pkg> precompile ※これが大事。addするたび必要。  
```
* 変数や関数の定義をリセット  
```Julia
julia> workspace()  
```

- Plotsは別でインストールするといいかも(他のパッケージでも応用可能)  
```Julia
(v1.0) pkg> add https://github.com/JuliaPlots/Plots.jl.git
```

* PyPlotと、Plotsは共存させないほうがいいかも  

## 参考サイト
- [WindowsでJupyter notebookにJulia v1.0を追加してHello,Worldするまでのメモ](https://qiita.com/SouTakenaka/items/ccfbb5a85330e97af70c)

- [ WindowsへのJulia言語のインストール(起動の確認等)](https://nbviewer.jupyter.org/gist/genkuroki/81de23edcae631a995e19a2ecf946a4f?flush_cache=true#Anaconda3%E3%81%A8Julia-v1.0%E3%81%AE%E7%B5%84%E3%81%BF%E5%90%88%E3%82%8F%E3%81%9B-(2018-09-05%E3%81%AB%E8%BF%BD%E5%8A%A0))

- [Juliaという速くて書きやすい言語をちょっとだけ覗いてみたんだが、なにやらワクワクするものがあったので報告しようと思う](https://qiita.com/sadayuki-matsuno/items/fc5e9ec3894a4b7bfbfb)
