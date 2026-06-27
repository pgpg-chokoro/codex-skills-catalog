# Bug Museum Curator

## Metadata

| Field | Value |
|---|---|
| Category | Fun |
| Difficulty | Beginner |
| Estimated time | 20-45 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Issue tracker, postmortems, incident notes |
| Tags | fun, bug, incident, learning |

## Purpose

過去の不具合や障害を、博物館展示のように整理し、学習資産として残す。

## Use Cases

- 新人研修
- 障害共有会
- 開発者イベント
- プロジェクトの歴史整理

## Inputs

- Issue
- 障害報告書
- 修正PR
- 学んだ教訓

## Workflow

1. 代表的な不具合を収集する。
2. 発生原因と影響を整理する。
3. 修正内容を要約する。
4. 展示カードとして再構成する。
5. 学習ポイントを抽出する。

## Outputs

- `museum-catalog.md`
- `exhibit-cards.md`
- `lessons-learned.md`

## Implementation Idea

埋もれがちな障害報告を、読みやすく印象に残る教材へ変換する。

## Example

設定名の typo による通知停止を、原因、検出方法、再発防止策の展示カードとしてまとめる。

## Future Improvements

- Incident Replay Builderとの連携
- 展示カードテンプレート追加
- 重要度別分類
