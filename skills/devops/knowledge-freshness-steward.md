# Knowledge Freshness Steward

## Metadata

| Field | Value |
|---|---|
| Category | DevOps |
| Difficulty | Intermediate |
| Estimated time | 30-90 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Documentation, repositories, runbooks |
| Tags | devops, documentation, knowledge-base, rag |

## Purpose

社内ドキュメント、Runbook、設計資料、AI向け知識ベースの陳腐化を検出する。

## Use Cases

- RAGの知識ベースを運用しているとき
- オンボーディング資料が古くなりやすいとき
- 実装とドキュメントの差分を確認したいとき

## Inputs

- ドキュメント群
- ソースコード
- API仕様
- Runbook

## Workflow

1. 文書を収集し、参照先や用語を抽出する。
2. コードや設定と整合しているか確認する。
3. 廃止済み要素や存在しないサービスへの参照を検出する。
4. 更新優先度を付ける。
5. 修正提案を作成する。

## Outputs

- `freshness-report.md`
- `stale-content-list.md`
- `update-priority.md`

## Implementation Idea

ドキュメントとリポジトリを横断検索し、古いAPI名、削除済み設定、実装と異なる手順を検出する。

## Example

READMEに旧デプロイコマンドが残っている場合、現在のCI/CD設定との差分を示して更新案を出す。

## Future Improvements

- ドキュメント更新PRの自動作成
- RAG検索ログからの不足知識検出
- 文書鮮度スコアのダッシュボード化
