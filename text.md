# よく使うgitコマンド

## ローカルリポジトリでよく使うコマンド

### initコマンド
リポジトリを新規作成する
```
＃新しくプロジェクト作成する場合
git init 
```

### configコマンド
現在の設定を取得、変更する
```
git config 
```

### addコマンド
変更内容をインデックスに追加してコミット対象にする

```
git add ファイル名
# 実務では変更を全て含めるため"."を使っている
git add .
```

### commitコマンド 
インデックスの現在の内容と変更を説明する指定されたログメッセージを含む新しいコミットを作成
<br> 
https://tracpath.com/docs/git-commit/

```
git commit -m "コミットメッセージ"

```

### logコマンド

コミットログを表示する

```
git log 
# コミットログを１行で確認した場合
git log --oneline
```

### statusコマンド
作業ツリーのステータスを表示する
```
git status 
```

### branchコマンド
ブランチの一覧を出力したり、削除、名前の変更が行える。

```
# ブランチの一覧表示
git branch

# ブランチの削除
git branch rm <ブランチ名>

```

### checkoutコマンド
作業ツリーを異なるブランチに切り替える

```
git checkout <ブランチ名>
# ブランチの作成 
git checkout -b <ブランチ名>

```

### mergeコマンド
他のブランチやコミットの内容を現在のブランチに取り込む
```
git merge <ブランチ名>
```

### resetコマンド
ファイルをインデックスから削除し、特定のコミットの状態まで戻す<br/>


|  オプション  |  意味  |
| ---- | ---- |
|  --hard  |  add、commit、ワーキングツリーの取り消し  |
|  --mixed  | add、commitの取り消し |
| --soft | commitのみ取り消し |
```

# 直前のコミットをなかったことにする
git reset --soft HEAD^

# 直前のコミットを取り消し
git reset --hard HEAD^

# コミット後の変更を全部消したい
git reset --hard HEAD

# addを取り消したい
git reset --mixed HEAD

# git resetをなかったことにする
git reset --hard ORIG_HEAD
```

## リモートリポジトリとローカルリポジトリでやりとりする際に使うコマンド 

### remoteコマンド
リモートリポジトリを関連付けする
```
# リモートリポジトリを追加
git remote add <githubのURL>

# リモートリポジトリを削除
git remote rm <リモートリポジトリ名>

# リモートリポジトリの一覧表示
git remote 

```

### pushコマンド
ローカルリポジトリの変更内容をリモートリポジトリに送信する
```
git push <リモートリポジトリ名> <ブランチ名>
```

### pullコマンド
リモートリポジトリの内容を取得し、現在のブランチに取り込む（「fetch」と「merge」を行う）
```
git pull <リモートリポジトリ名> <ブランチ名>
```

### cloneコマンド
リポジトリのクローンを作成する
```
git clone "リポジトリURL"
＃ 口頭で説明
```
