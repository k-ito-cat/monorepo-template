# Structure Steering

## この文書の役割

この文書は、アーキテクチャとディレクトリ設計を定義するための仕様書である。  
ここでは、責務分割、依存方向、ディレクトリ設計、レイヤ構成を扱う。  

## 現在の主要構成

```txt
docs/
  AGENTS.md
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
    glossary.md
  diagrams/.gitkeep
  pencil/.gitkeep
```

## 現在のディレクトリ設計

- `docs/design`
- デザイン文書群の配置場所
- 上位原則、foundations、layouts、components、patterns、screens、tokens、checklist をまとめて扱う

- `docs/diagrams`
- ER 図などの図を置く

- `docs/pencil`
- 補助素材を置く

- `docs/specs`
- プロダクト、用語、技術、構成、API の仕様書

- `docs/specs/glossary.md`
- UI と API の表示語彙、および DB スキーマとの対応関係を定義する正本
- 命名の表記ゆれを防ぐ基準
