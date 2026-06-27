# Incident Replay Builder

## Metadata

| Field | Value |
|---|---|
| Category | DevOps |
| Difficulty | Advanced |
| Estimated time | 45-120 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Incident report, logs, metrics, commits |
| Tags | devops, incident, sre, testing |

## Purpose

本番障害やインシデントの記録から、再現可能な検証シナリオと再発防止テストを作成する。

## Use Cases

- 障害対応後の振り返りを行うとき
- 原因分析をテスト資産へ変換したいとき
- 同じ障害の再発をCIで防ぎたいとき

## Inputs

- インシデントレポート
- アプリケーションログ
- メトリクス
- 関連コミット

## Workflow

1. インシデントのタイムラインを抽出する。
2. 発生条件と影響範囲を整理する。
3. 最小再現シナリオを作る。
4. 回帰テスト案を生成する。
5. 再発防止策を運用チェックリストに落とし込む。

## Outputs

- `replay-scenario.md`
- `regression-tests/`
- `prevention-plan.md`

## Implementation Idea

障害報告書とログを入力し、再現条件、期待される失敗、修正後に通るべきテストケースを生成する。

## Example

特定の環境変数欠落でジョブが停止した障害を、設定検証テストと起動前チェックへ変換する。

## Future Improvements

- ログからの自動タイムライン生成
- テストコードの自動PR化
- Synthetic Incident Simulatorとの連携
