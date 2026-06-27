# Repository Storyteller

## Metadata

| Field | Value |
|---|---|
| Category | Fun |
| Difficulty | Beginner |
| Estimated time | 20-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Git history, pull requests, release notes |
| Tags | fun, git, storytelling, onboarding |

## Purpose

Git履歴を物語、ドキュメンタリー、学習ガイドとして再構成する。

## Use Cases

- プロジェクト周年企画
- OSS紹介
- オンボーディング
- コミット設計の学習

## Inputs

- Git log
- Pull Request
- Release notes
- 主要な開発イベント

## Workflow

1. 主要な変更イベントを抽出する。
2. 開発フェーズを分類する。
3. 転換点を見つける。
4. 物語形式または教材形式に変換する。
5. 学びと印象的な場面をまとめる。

## Outputs

- `project-story.md`
- `project-timeline.md`
- `learning-questions.md`

## Implementation Idea

Software Evolution Documentary、Commit Message Novelist、Git History Story Guide を統合したSkillとして扱う。

## Example

大規模リファクタリングを「静かな土台作り」の章として描き、後の開発速度向上との関係を説明する。

## Future Improvements

- リリースノート自動生成
- 新人向け学習ルート作成
- 技術的転換点の自動検出
