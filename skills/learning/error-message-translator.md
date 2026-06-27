# Error Message Translator

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 10-25 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Error message, stack trace, source code |
| Tags | learning, debugging, error, beginner |

## Purpose

エラーメッセージを初心者向けの学習ガイドに変換する。

## Use Cases

- PythonやJavaScriptの学習中にエラーで詰まったとき
- スタックトレースの読み方を学びたいとき
- 同じエラーを再発させない調査手順を知りたいとき

## Inputs

- エラーメッセージ
- スタックトレース
- 関連コード
- 実行環境

## Workflow

1. エラーの種類を分類する。
2. 直接原因と根本原因の候補を分ける。
3. 調査順序を説明する。
4. 修正例を提示する。
5. 再発防止の考え方を説明する。

## Outputs

- `error-guide.md`
- `debugging-checklist.md`
- `fixed-example.md`

## Implementation Idea

エラー文を単に翻訳せず、どの行を見るべきか、何を確認すべきか、どう直すかを順番に示す。

## Example

`TypeError: Cannot read properties of undefined` を、未定義値の発生箇所、入力確認、nullチェックの考え方へ分解する。

## Future Improvements

- フレームワーク別エラー辞書
- IDEログとの連携
- 類似エラーの学習カード生成
