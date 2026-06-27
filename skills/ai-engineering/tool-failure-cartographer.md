# Tool Failure Cartographer

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Advanced |
| Estimated time | 45-90 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Agent logs, tool outputs, incident notes |
| Tags | ai-engineering, agent, tools, reliability |

## Purpose

AIエージェントが使うAPI、CLI、DB、ブラウザ操作などの失敗パターンを地図化し、回復戦略を構築する。

## Use Cases

- 長時間エージェント実行の成功率を上げたいとき
- MCPツールや外部APIの失敗が多いとき
- ツール障害からの復帰手順を標準化したいとき

## Inputs

- 実行ログ
- ツール出力
- エラー履歴
- 既存の回復手順

## Workflow

1. ログからツール失敗を抽出する。
2. 失敗を認証、ネットワーク、入力不備、権限、仕様変更などに分類する。
3. 失敗の連鎖や頻度を分析する。
4. 有効だった回復策を抽出する。
5. リトライ方針とプレイブックを作成する。

## Outputs

- `failure-map.md`
- `recovery-playbook.md`
- `resilience-report.md`

## Implementation Idea

エージェント実行ログを定期的に解析し、失敗理由と復旧手順をナレッジ化する。

## Example

GitHub APIのレート制限、ブラウザ操作の要素未検出、CLIコマンドの権限不足を別々の回復パターンとして管理する。

## Future Improvements

- 自動リトライポリシー生成
- 失敗確率の時系列分析
- ツールごとの健全性スコア化
