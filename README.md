## monorepo-template

アプリケーションコード用の monorepo ひな形。

## docs

このリポジトリは docs の実体を持たない。

docs は private repository の `project-documents/<project>/` に作成し、プロジェクト側では symlink を貼る。

```text
<project>/
  docs -> ../project-documents/<project>
```

docs ひな形の正本は `project-documents/_template/`。

## 主要スクリプト

```sh
corepack enable
```
