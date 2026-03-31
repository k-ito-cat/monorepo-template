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
