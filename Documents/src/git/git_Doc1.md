# git 備忘録

## gitコマンドでgithubにpushするまで(簡潔版)

1. ファイルをステージに追加
```
git add . // すべてのファイル、ディレクトリ
```

2. ファイルをコミット
git commit -m "コミット文"

3. リモートにプッシュ
git push origin master  //masterを更新

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
