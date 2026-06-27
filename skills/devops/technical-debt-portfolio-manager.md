# Technical Debt Portfolio Manager

## Metadata

| Field | Value |
|---|---|
| Category | DevOps |
| Difficulty | Intermediate |
| Estimated time | 45-90 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Source code, issue tracker, architecture notes |
| Tags | devops, technical-debt, planning, refactoring |

## Purpose

技術的負債を単なるTODOではなく、コスト、リスク、影響範囲、価値を持つポートフォリオとして管理する。

## Use Cases

- 四半期の開発計画を立てるとき
- リファクタリング対象を選ぶとき
- 技術的負債の説明責任を高めたいとき

## Inputs

- ソースコード
- IssueやTODO
- 障害履歴
- アーキテクチャメモ

## Workflow

1. 技術的負債候補を抽出する。
2. 修正コストを見積もる。
3. 将来リスクと影響範囲を評価する。
4. 改善による価値を整理する。
5. 優先順位とロードマップを作る。

## Outputs

- `debt-portfolio.md`
- `priority-matrix.md`
- `refactoring-roadmap.md`

## Implementation Idea

Issue、コードスメル、障害履歴を統合し、「今返済すべき負債」と「後回しでよい負債」を分類する。

## Example

巨大クラス、未更新依存関係、テスト不足を比較し、障害リスクと修正コストから優先度を決める。

## Future Improvements

- コードメトリクスとの連携
- 事業影響度の定量化
- ロードマップ管理ツールとの同期
