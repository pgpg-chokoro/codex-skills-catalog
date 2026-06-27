# Release Readiness Orchestrator

## Metadata

| Field | Value |
|---|---|
| Category | DevOps |
| Difficulty | Intermediate |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Release notes, test results, deployment plan |
| Tags | devops, release, checklist, operations |

## Purpose

リリース直前に必要な確認事項を横断的に収集し、リリース可否を判断する。

## Use Cases

- SaaSやAIプロダクトの本番リリース前
- モデル切り替えや重要機能公開の前
- 確認漏れを減らしたいとき

## Inputs

- リリースノート
- テスト結果
- デプロイ手順
- 監視・通知設定
- ロールバック計画

## Workflow

1. 変更内容を整理する。
2. テストとレビューの完了状況を確認する。
3. ドキュメント更新と運用準備を確認する。
4. 監視項目とロールバック条件を確認する。
5. Go / No-Go 判定を出す。

## Outputs

- `release-readiness.md`
- `launch-checklist.md`
- `risk-register.md`

## Implementation Idea

リリースPRやリリースノートを読み、未完了チェック、リスク、ロールバック可否をまとめる。

## Example

新しいモデルを本番投入する前に、評価結果、段階公開計画、監視指標、戻し手順を確認する。

## Future Improvements

- CI/CDとの連携
- Feature Flag Rollout Plannerとの連携
- リリース後レビューの自動生成
