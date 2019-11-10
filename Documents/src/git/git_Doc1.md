# git 備忘録

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
