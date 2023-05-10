## git clone

![git-clone](https://github.com/dev-nakasho/udemy-git/assets/40833446/c8be0479-8e26-4535-83eb-c003b9b908e5)

```shell
git clone <repository_url>
```

## git branch, git checkout

![git-branch](https://github.com/dev-nakasho/udemy-git/assets/40833446/222bd94e-dc76-4c3e-9645-e64b60318dfc)

```shell
# ブランチ一覧
git branch
git branch -a

# ブランチ作成
git checkout -b new_branch_name

# リモートブランチからローカルブランチを作成
git checkout -t new_branch_name

# ブランチ削除
git branch -D branch_name
```

## git status, git add, git commit, git reset, git push

![git-status](https://github.com/dev-nakasho/udemy-git/assets/40833446/918bc665-2c27-4577-8a52-246c8bfac31b)

```shell
# 状態確認
git status

# インデックス（ステージングに追加)
git add .

# コミット
git commit -m "commit_message"

# リセット
git reset --soft HEAD^
git reset --hard HEAD^
git reset file_name
git checkout .

# 直前のコミットに変更を追加する新しいコミットを作成
git commit --amend

# ローカルの変更をリモートリポジトリへ反映
git push origin HEAD

# ブランチの移動
git checkout branch_name
git checkout -
```

## git fech, git pull

```shell
# リモートリポジトリから最新情報を取得
git fetch

# fetch + 削除済みのリモートリポジトリを削除
git fetch -p

# fetch + ローカルリポジトリにマージ
git pull
```

## git stash, git log, git show

```shell
# 作業内容を一時退避
git stash

# 未追跡のファイルも併せて退避
git stash -u

# 退避した作業内容を復元 + 退避内容を削除
git stash pop

# コミット履歴を確認
git log

# 特定のコミット詳細を確認
git show commit_id
```
