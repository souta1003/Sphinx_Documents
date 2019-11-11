# git 備忘録



## gitコマンドでgithubにpushするまで(簡潔版)

1. ファイルをステージに追加
```
git add . // すべてのファイル、ディレクトリ
```

2. ファイルをコミット
```
git commit -m "コミット文"
```

3. リモートにプッシュ
```
git push origin master  //masterを更新
```

### 参考サイト
- [【Git】基本コマンド](https://qiita.com/konweb/items/621722f67fdd8f86a017)



## リモートのファイルを消す方法

1. ファイルを消す
```git
git rm -r --cached Documents/.vscode
```
2. 前ステージと比較して変更点があった部分のみadd
```git
git add -u
```
3. コミット
```git
git commit -m ".vscode Del"
```
4. プッシュ
```git
git push origin master
```

### 参考サイト
・[【Git】ファイルをローカルには残してリモートリポジトリからのみ削除](http://mimaunes.hatenablog.com/entry/20150817/1439741937)



## git管理からディレクトリを外す方法

1. workspace直下で「新しいファイル」アイコンを押し、「.gitignore」を生成。

2. 「.gitignore」ファイルを編集。
```.gitignore
.vscode/
_build/
```

### 参考サイト
[Visual studio codeで.vscodeディレクトリをgit管理から外す](https://qiita.com/EngTks/items/a4f875956f0b087668f6)



## GitでProxyの設定を行ってエラー回避する方法

1. 環境設定ファイルの設定

   コマンドプロンプトで以下を入力。

    (設定ファイルの位置は、Windowsの環境ではユーザディレクトリ配下の「.gitconfig」ファイル) 

```bash
git config --global http.proxy http://proxy.ほにゃらら.co.jp:8080
git config --global https.proxy http://proxy.ほにゃらら.co.jp:8080
```

2. 設定されているか確認

```bash
git config --list
```

### 参考サイト

- [GitでProxyの設定を行ってエラー回避する方法]( https://git-manual.net/git-proxy-error/ )

