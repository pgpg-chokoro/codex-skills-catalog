# Dependency Upgrade Navigator

## Metadata

| Field | Value |
|---|---|
| Category | DevOps |
| Difficulty | Intermediate |
| Estimated time | 30-90 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Dependency manifests, changelogs, tests |
| Tags | devops, dependency, maintenance, testing |

## Purpose

依存ライブラリやフレームワークの更新について、破壊的変更、影響範囲、移行計画、ロールバック方針を整理する。

## Use Cases

- DependabotやRenovateのPRをレビューするとき
- メジャーバージョンアップを計画するとき
- セキュリティ修正を安全に取り込むとき

## Inputs

- `package.json`、`requirements.txt`、`pom.xml` など
- 変更対象バージョン
- リリースノート
- テスト結果

## Workflow

1. 更新対象と差分を抽出する。
2. Breaking Change候補を確認する。
3. 影響を受けるコードと設定を探す。
4. 移行タスクを段階分解する。
5. テスト強化案とロールバック手順を作る。

## Outputs

- `upgrade-plan.md`
- `risk-analysis.md`
- `migration-checklist.md`

## Implementation Idea

依存関係更新PRに対して自動実行し、リリースノート要約、影響ファイル候補、必要テストをコメントとして生成する。

## Example

FastAPIやReactのメジャーバージョン更新で、非推奨API、型定義変更、設定変更を洗い出す。

## Future Improvements

- Renovate / Dependabot との連携
- CI失敗ログの自動解析
- 依存関係ごとの更新リスクスコア化
