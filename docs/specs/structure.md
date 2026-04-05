# Structure Steering

## この文書の役割

この文書は、アーキテクチャとディレクトリ設計を定義するための仕様書である。  
ここでは、責務分割、依存方向、ディレクトリ設計、レイヤ構成を扱う。  

## 現在の主要構成

```txt
.codex/
  AGENTS.md
docs/
  design/
    DESIGN.md
    foundations.md
    layouts.md
    components.md
    ui-patterns.md
    screens.md
    tokens.md
    checklist.md
  specs/
    product.md
    glossary.md
    tech.md
    structure.md
    api.md
    nfr.md
    qa.md
    research.md
    implementation-plan.md
    release.md
    legal.md
  diagrams/.gitkeep
  pencil/.gitkeep
```

## 現在のディレクトリ設計

- `.codex`
- AI 向け運用ルールの配置場所
- `AGENTS.md` など、プロジェクト全体の指示を管理する

- `docs/design`
- デザイン文書群の配置場所
- 上位原則、foundations、layouts、components、patterns、screens、tokens、checklist をまとめて扱う

- `docs/diagrams`
- ER 図などの図を置く

- `docs/pencil`
- 補助素材を置く

- `docs/specs`
- プロダクト、用語、技術、構成、API の仕様書

- `docs/specs/product.md`
- 背景、対象ユーザー、提供価値、ゴール、スコープを定義する正本

- `docs/specs/glossary.md`
- UI と API の表示語彙、および DB スキーマとの対応関係を定義する正本
- 命名の表記ゆれを防ぐ基準

- `docs/specs/tech.md`
- 技術選定、技術方針、未決事項を定義する正本

- `docs/specs/api.md`
- API 契約、入出力、エラー方針を定義する正本

- `docs/specs/nfr.md`
- 非機能要件、対応環境、運用要件を定義する正本

- `docs/specs/qa.md`
- 受け入れ基準、テスト観点、回帰観点を定義する正本

- `docs/specs/research.md`
- 調査結果、比較観点、採用理由の記録先

- `docs/specs/implementation-plan.md`
- Do / Later / Skip と MVP 実装計画を管理する文書

- `docs/specs/release.md`
- リリース準備、CI/CD、公開前チェックを管理する文書

- `docs/specs/legal.md`
- 法務、プライバシー、同意設計の整理先
