# 実践

## プロジェクト管理の始め方

### リモートリポジトリをクローンする

```
git clone https://github.com/kazutotakeuchi-32/git_test.git
```

### ローカルリポジトリからプロジェクトを作成するフロー

```
git init
git add .
git commit -m "first commit"
git remote add origin 
git push origin main
```

## ローカルリポジトリの作業

### 新しくgitで管理を始める

```
git init
```

### 新規ブランチを作成

```
# 1.現在のブランチを確認
git branch
# 2. 差分を確認
git diff 
# 3.ブランチを作成
git checkout -b test1
# 4.ブランチ確認
git branch
```

### 変更した内容コミットする
```
git add .
git commit 
```
## リモートリポジトリとやりとりする

### ローカルリポジトリの変更をリモートリポジトリに共有するフロー

```
git add .
git commit -m "メッセージ"
git push origin main
```

### リモートリポジトリの変更をローカルリポジトリに取り込む

```
# 差分を確認
git stauts 
git pull origin main
```

