# takatomo/.github

個人アカウント配下リポジトリ向けのデフォルトコミュニティヘルスファイル置き場です。

- PR テンプレート: `.github/PULL_REQUEST_TEMPLATE.md`
- Issue テンプレート（Parent/Child運用）:
  - `.github/ISSUE_TEMPLATE/feature.yml`（Parent Issue向け）
  - `.github/ISSUE_TEMPLATE/task.yml`（Child Issue向け）
  - `.github/ISSUE_TEMPLATE/bug.yml`（不具合報告。必要に応じてParent Issueへ紐付け）
- Issue テンプレート設定: `.github/ISSUE_TEMPLATE/config.yml`（`blank_issues_enabled: true`）

このリポジトリは、各リポジトリに同名ファイルがない場合の既定値として使われます。

## 運用方針（Parent-Child）

- 親となる課題は Parent Issue として起票する
- 実装単位は Child Issue として起票し、Parent Issue に紐付ける
- Featureテンプレートは Parent Issue 起票用、Taskテンプレートは Child Issue 起票用として使う
- Bugテンプレートは単独修正でも Parent Issue 配下でも使える

## PRの関連Issue記載ルール

- Parent Issue は `Refs #<Parent番号>` で記載する（自動クローズはしない）
- Child Issue は `Closes #<Child番号>` または `Fixes #<Child番号>` で記載する（自動クローズされる）
- Child Issue が複数ある場合は `Closes #...` / `Fixes #...` を複数行で列挙する
- Parent Issue を Linked issues に表示したい場合は、PR右ペインの `Development` から Parent Issue を手動リンクする
