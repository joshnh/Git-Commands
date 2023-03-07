Git コマンド集
============

## 翻訳バージョン
- [English version (original)](https://github.com/shion1305/Git-Commands/blob/master/README.md)
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)

___

_よく使われるGit Command集_

Gitエイリアスについては、以下の `.bash_profile` を参照してください。
*https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### プロジェクトの作成と取得

| Command | Description |
| ------- | ----------- |
| `git init` | Gitレポジトリの初期化。 |
| `git clone ssh://git@github.com/[ユーザー名]/[repository-name].git` | リモートレポジトリをローカルにクローン。 |

### 基本的な操作

| Command | Description |
| ------- | ----------- |
| `git status` | 現在の状況を確認。 |
| `git add [ファイル名]` | ステージングエリアにファイルを追加。 |
| `git add -A` | ステージングエリアに、全ての新規・変更ファイルを追加。 |
| `git commit -m "[コミットメッセージ]"` | 変更をコミット。 |
| `git rm -r [ファイル名]` | ファイル・フォルダーをステージングエリアから削除。 |

### ブランチの操作とマージ

| Command | Description |
| ------- | ----------- |
| `git branch` | ブランチの一覧を表示。(\*アスタリスクは現在のブランチを示す) |
| `git branch -a` | 全てのブランチの一覧を表示。(リモートを含む) |
| `git branch [ブランチ名]` | 新しいブランチを作成。 |
| `git branch -d [ブランチ名]` | ブランチを削除。 |
| `git push origin --delete [ブランチ名]` | リモート上のブランチを削除。 |
| `git checkout -b [ブランチ名]` | 新しいブランチを作成して切り替え。 |
| `git checkout -b [ブランチ名] origin/[ブランチ名]` | リモートブランチをクローンして切り替え。 |
| `git branch -m [old ブランチ名] [new ブランチ名]` | ブランチの名前を変更。 |
| `git checkout [ブランチ名]` | ブランチを切り替え。 |
| `git checkout -` | 最後に使ったブランチに切り替え。 |
| `git checkout -- [ファイル名]` | 指定したファイルの変更を破棄。 |
| `git merge [指定のブランチ名]` | 指定したブランチを現在のブランチにマージ。 |
| `git merge [指定のブランチ名] [対象のブランチ名]` | 指定したブランチを対象のブランチにマージ。 |
| `git stash` | 現在の変更を退避。 |
| `git stash clear` | 全ての退避した変更を消去。 |

### プロジェクトの共有と更新

| Command | Description |
| ------- | ----------- |
| git push origin [ブランチ名] | ブランチをリモートリポジトリにプッシュ。 |
| git push -u origin [ブランチ名] | 変更をリモートリポジトリにプッシュ。(指定したリモートブランチをデフォルトとして設定) |
| git push | 変更をリモートリポジトリにプッシュ。(デフォルトのブランチ) |
| git push origin --delete [ブランチ名] | 指定したリモートブランチを削除。 |
| git pull | ローカルリポジトリを最新のコミットに更新。 |
| git pull origin [ブランチ名] | リモートリポジトリから変更を取得。 |
| git remote add origin ssh://git@github.com/[ユーザー名]/[リポジトリ名].git | リモートリポジトリを追加。 |
| git remote set-url origin ssh://git@github.com/[ユーザー名]/[リポジトリ名].git | リポジトリのoriginブランチをSSHに設定。 |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | 変更履歴を確認。 |
| `git log --summary` | 詳細な変更履歴を確認。 |
| `git log --oneline` | 簡略化された変更履歴を確認。 |
| `git diff [元のブランチ] [対象のブランチ]` | マージする前に変更をプレビュー。 |
