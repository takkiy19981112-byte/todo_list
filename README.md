# TODOリストの公開手順（GitHub Pages）

このプロジェクトは `index.html` だけで動く静的サイトです。
以下の手順で無料公開できます。

1. GitHubで新しいリポジトリを作成
2. このフォルダの内容を `main` ブランチにpush
3. GitHubリポジトリの `Settings` -> `Pages` -> `Build and deployment` で `Source` を `GitHub Actions` に設定
4. `Actions` タブで `Deploy static site to GitHub Pages` が成功するのを待つ
5. 公開URL `https://<GitHubユーザー名>.github.io/<リポジトリ名>/` を開く

## 初回pushの例

```bash
git init
git add .
git commit -m "Add TODO app and GitHub Pages deployment"
git branch -M main
git remote add origin https://github.com/<GitHubユーザー名>/<リポジトリ名>.git
git push -u origin main
```
