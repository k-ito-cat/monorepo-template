# Validation Steering

## この文書の役割

この文書は、validation の正本をコードに置く前提で、コードだけでは共有しづらい判断だけを補足するための文書である。  
制約の詳細は zod schema と OpenAPI を正本とし、この文書では責務分担と未決事項だけを扱う。  

## 基本方針

- API 契約として表現できる制約は zod schema に書く
- OpenAPI は zod schema から生成し、手書きで二重管理しない
- FE と API で共有する制約は `packages/shared` に置く
- HTTP 固有の path param / query param / header の制約は `apps/api` 側で持つ
- UI 入力中の一時状態に依存する検証は `apps/web` 側で持つ
- DB 制約で担保する内容は DB 側に寄せる

## この文書に残すこと

- zod / OpenAPI だけでは表現しづらい責務分担
- FE 入力中検証と API 境界検証の差分
- normalize や前処理の方針
- 一意性や参照整合性のような非同期 / 永続化依存の扱い
- 未決事項

## 先に決める論点

- FE と API で共有する zod schema の範囲
  - 状態: 未定
  - メモ:

- 空文字 / `null` / `undefined` の扱い
  - 状態: 未定
  - メモ:

- trim / normalize の有無
  - 状態: 未定
  - メモ:

- 一意性チェックをどの層で担保するか
  - 状態: 未定
  - メモ:

- DB 制約に任せるものと API で先に弾くものの切り分け
  - 状態: 未定
  - メモ:

## 現時点で書かないこと

- 項目ごとの細かい length / pattern / enum 一覧
- OpenAPI にそのまま載る制約の再掲
- 実装済み schema の転記

## 未決事項

- 
