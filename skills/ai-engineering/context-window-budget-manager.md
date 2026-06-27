# Context Window Budget Manager

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Advanced |
| Estimated time | 20-45 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Repository access, document corpus, retrieval tools |
| Tags | ai-engineering, agent, context-management, retrieval |

## Purpose

大規模なコードベースやドキュメント群を扱う際に、限られたコンテキストウィンドウを最適配分する。

## Use Cases

- 巨大リポジトリをエージェントに読ませるとき
- 長時間タスクで重要情報が埋もれるとき
- 複数ドキュメントを参照するAIコードレビューを行うとき

## Inputs

- タスク目的
- 対象リポジトリまたは文書群
- 重要ファイル、制約、既知の判断材料

## Workflow

1. 情報源をコード、仕様、履歴、テスト、ドキュメントに分類する。
2. タスク達成に必要な情報の優先度を付ける。
3. その場で保持する情報、要約する情報、後で再取得する情報を分ける。
4. コンテキストに入れる順番を設計する。
5. 欠落リスクと再取得戦略を記録する。

## Outputs

- `context-plan.md`
- `compression-report.md`
- `retrieval-map.md`

## Implementation Idea

エージェント実行前に、タスク目的とリポジトリ構造を渡して、読み込むべきファイル群と要約方針を生成させる。

## Example

大規模Webアプリで認証機能を修正する際、認証ミドルウェア、ルーティング、テスト、設定ファイルを優先的に保持する。

## Future Improvements

- トークン数推定の自動化
- 実行途中でのコンテキスト再構成
- 重要情報の抜け漏れ検出
