# Gitの勉強会
6月時に社内勉強会で使うリポジトリ

## 全体の流れ
- 簡単な自己紹介 5分（初めましての人がいた場合）
- 自分がレクチャ- 10〜15分
- 自由時間・質疑応答 30〜分
- まとめ (アンケートを含む）5分

## 事前準備
- gitHubアカウントの作成
- gitコマンドをインストール

## 内容
もしかすると１勉強会で1セクションになる可能性があり？
1. 基礎的なgitコマンドの操作
2. githubでPRを出してみよう
3. コンフリクトを解決してみよう
4. まとめ

### 1. 基礎的なgitコマンドの操作
参加者に資料を共有。<br>
実際に実行してもらう。<br>
画面共有上では自分がコマンドを実行し、どのような時にそのコマンドを使うかを<br>
簡単に説明。
```
  git log 
　git checkout -b ブランチ名
  git branch
  git remote 
  git branch -m "変更したいブランチ名"
  git diff
  git add ファイル名
  git commit -m "コミットメッセージ"
  git push origin ブランチ名
  git pull origin ブランチ名
```
### 2. githubでPRを出してみよう
参加者事にブランチを切ってもらい、pushコマンドを使ってリモートリポジトリにローカルリポジトリの <br>
変更を反映する。
### 3. コンフリクトを解決してみよう
同じブランチ内で同じファイルに変更を加えて意図的にコンフリクトを起こす。<br>
git hubでコンフリクトを解消してみる。(代表者)

### 4. まとめ
勉強会で学んだことの振り返り<br>
質疑応答。


## 資料
- [よく使うgitコマンド](https://github.com/kazutotakeuchi-32/git_test/blob/main/text.md)
- [実践](https://github.com/kazutotakeuchi-32/git_test/blob/main/text2.md)

