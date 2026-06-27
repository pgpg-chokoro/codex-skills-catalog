# State Machine Coach

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 20-40 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Source code, workflow description |
| Tags | learning, state-machine, architecture, beginner |

## Purpose

複雑な処理を状態遷移図や遷移表として理解できるようにする。

## Use Cases

- 認証フローを理解したいとき
- 注文状態や申請ワークフローを学びたいとき
- 非同期処理やゲーム状態管理を理解したいとき

## Inputs

- 対象コード
- ユースケース
- イベントや状態の説明

## Workflow

1. 状態候補を抽出する。
2. 状態を変えるイベントを抽出する。
3. 遷移表を作る。
4. 正常系と異常系を分ける。
5. 状態遷移図と練習問題を作る。

## Outputs

- `state-diagram.md`
- `transition-table.md`
- `exercises.md`

## Implementation Idea

コードや仕様から状態、イベント、遷移条件を抽出し、初心者向けの説明と図解用テキストに変換する。

## Example

注文管理で `created -> paid -> shipped -> delivered` の遷移と、キャンセルや返金の例外遷移を整理する。

## Future Improvements

- Mermaid図の自動生成
- 不正遷移の検出
- テストケース生成との連携
