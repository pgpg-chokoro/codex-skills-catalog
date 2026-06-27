# Synthetic Incident Simulator

## Metadata

| Field | Value |
|---|---|
| Category | DevOps |
| Difficulty | Advanced |
| Estimated time | 45-120 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Architecture docs, dependency map, runbooks |
| Tags | devops, incident, sre, resilience |

## Purpose

実際にはまだ発生していない障害シナリオを生成し、運用耐性を高める。

## Use Cases

- AIプロダクトの運用訓練をしたいとき
- API停止、モデル障害、検索品質劣化などを事前に想定したいとき
- Runbookの穴を発見したいとき

## Inputs

- システム構成図
- 外部依存サービス
- 既存Runbook
- 監視項目

## Workflow

1. 障害候補を生成する。
2. 障害の連鎖と影響範囲を推定する。
3. 現在の対応手順で復旧可能か評価する。
4. 足りない監視、通知、手順を特定する。
5. 改善案を作成する。

## Outputs

- `incident-scenarios.md`
- `response-checklist.md`
- `resilience-improvements.md`

## Implementation Idea

アーキテクチャと依存関係を入力し、起こり得る障害を複数生成して、机上訓練用のシナリオへ変換する。

## Example

LLM APIが高レイテンシになった場合、フォールバック、タイムアウト、ユーザー通知、SLOへの影響を確認する。

## Future Improvements

- Chaos Engineeringツールとの連携
- 障害発生確率の見積もり
- Runbook更新PRの自動生成
