# Data Contract Guardian

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Intermediate |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Schemas, API specs, consumer list |
| Tags | ai-engineering, data, schema, compatibility |

## Purpose

サービス間・パイプライン間のデータ契約を監視し、破壊的変更や互換性問題を事前検出する。

## Use Cases

- APIやイベントスキーマを変更するとき
- ETLや特徴量パイプラインを更新するとき
- 下流サービスへの影響を確認したいとき

## Inputs

- 旧スキーマ
- 新スキーマ
- Consumer一覧
- サンプルデータ

## Workflow

1. スキーマ差分を抽出する。
2. Breaking Change候補を分類する。
3. 下流利用者への影響を推定する。
4. 移行方針を作成する。
5. Contract Test案を生成する。

## Outputs

- `compatibility-report.md`
- `migration-guide.md`
- `contract-tests.md`

## Implementation Idea

JSON Schema、OpenAPI、protobuf、Parquetスキーマなどを比較し、必須フィールド削除や型変更を検出する。

## Example

イベントの `user_id` が数値から文字列に変わる場合、下流集計処理や特徴量生成処理への影響を洗い出す。

## Future Improvements

- OpenAPI差分ツールとの連携
- Consumer別の影響度スコア
- テストコード自動生成
