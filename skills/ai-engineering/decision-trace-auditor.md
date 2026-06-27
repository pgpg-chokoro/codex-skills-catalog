# Decision Trace Auditor

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Advanced |
| Estimated time | 45-90 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Agent execution logs, tool invocations, outputs |
| Tags | ai-engineering, agent, governance, auditability |

## Purpose

AIエージェントや自動化システムの判断過程を追跡し、監査可能な形で整理する。

## Use Cases

- エージェントがなぜ失敗したかを説明したいとき
- 高信頼なAIシステムで判断根拠を残したいとき
- ツール選択や分岐判断をレビューしたいとき

## Inputs

- 実行ログ
- ツール呼び出し履歴
- 中間出力
- 最終成果物

## Workflow

1. 判断イベントを抽出する。
2. 判断に使われた根拠情報を紐づける。
3. 分岐点を時系列で整理する。
4. 誤った方向へ進んだ可能性のある地点を分析する。
5. 監査レポートと改善案を生成する。

## Outputs

- `decision-trace.md`
- `root-cause-map.md`
- `audit-summary.md`

## Implementation Idea

エージェントの実行ログから「どの情報を見て、どのツールを選び、どの判断に至ったか」を構造化する。

## Example

コード修正エージェントが誤ったファイルを編集した場合、検索クエリ、参照ファイル、判断理由を追跡して原因を特定する。

## Future Improvements

- 実行ログ形式の標準化
- 判断品質スコアの導入
- Tool Failure Cartographerとの連携
