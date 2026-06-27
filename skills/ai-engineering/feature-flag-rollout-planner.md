# Feature Flag Rollout Planner

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Intermediate |
| Estimated time | 20-45 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Feature description, monitoring metrics, rollout tool |
| Tags | ai-engineering, rollout, feature-flag, monitoring |

## Purpose

新機能やAI機能を安全に公開するため、フィーチャーフラグを使った段階的ロールアウト計画を作る。

## Use Cases

- AI機能を一部ユーザーにだけ公開したいとき
- モデル切り替えを段階的に行いたいとき
- A/Bテストや限定公開を設計したいとき

## Inputs

- 機能概要
- 対象ユーザー条件
- 監視するKPI
- ロールバック条件

## Workflow

1. 公開対象を定義する。
2. ロールアウト段階を設計する。
3. 監視指標としきい値を設定する。
4. ロールバック条件を明文化する。
5. 運用チェックリストを生成する。

## Outputs

- `rollout-plan.md`
- `monitoring-checklist.md`
- `rollback-playbook.md`

## Implementation Idea

新機能PRやリリースノートから公開範囲、段階、監視指標を抽出し、フラグ運用計画を生成する。

## Example

新しいAI要約機能を社内ユーザー、5%の顧客、25%、100%の順に公開し、エラー率や低評価率で停止判断を行う。

## Future Improvements

- Feature Flag SaaSとの連携
- KPI異常時の自動停止提案
- 実験結果の自動レポート化
