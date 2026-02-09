# takatomo/.github

個人アカウント配下リポジトリ向けのデフォルトコミュニティヘルスファイル置き場です。

- PR テンプレート: `.github/PULL_REQUEST_TEMPLATE.md`
- Issue テンプレート: `.github/ISSUE_TEMPLATE/*.yml`

このリポジトリは、各リポジトリに同名ファイルがない場合の既定値として使われます。

## 運用方針（Parent-Child）

- 親となる課題は Parent Issue として起票する
- 実装単位は Child Issue として起票し、Parent Issue に紐付ける
- PR では `Parent Issue: Refs #...` と `Child Issue: Closes #...` を併記する
