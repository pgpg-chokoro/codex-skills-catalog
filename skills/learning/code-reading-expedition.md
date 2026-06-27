# Code Reading Expedition

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Repository, learner level |
| Tags | learning, code-reading, oss, onboarding |

## Purpose

大きなコードベースをどこから、どの順番で読むべきか案内する。

## Use Cases

- OSSに初めて参加するとき
- インターンや新しいチームで既存コードを読むとき
- フレームワークやアプリの構造を理解したいとき

## Inputs

- リポジトリ
- 学習者のレベル
- 理解したい機能

## Workflow

1. エントリーポイントを特定する。
2. 主要モジュールを抽出する。
3. 実行経路を追跡する。
4. 読む順番と無視してよい箇所を示す。
5. 読解課題を作る。

## Outputs

- `reading-path.md`
- `architecture-notes.md`
- `exploration-tasks.md`

## Implementation Idea

リポジトリ構造を解析し、初心者が迷わず読める小さな探索ルートを作る。

## Example

Webアプリで、`main`、ルーティング、コントローラ、サービス、DBアクセスの順に読む道筋を示す。

## Future Improvements

- 実行トレースとの連携
- PR単位の読解ガイド
- オンボーディング資料化
