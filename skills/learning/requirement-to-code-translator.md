# Requirement-to-Code Translator

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 20-45 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Feature description, user stories |
| Tags | learning, requirements, design, implementation |

## Purpose

自然言語の要件を、データモデル、関数設計、モジュール分割、実装順序へ変換する練習を支援する。

## Use Cases

- 個人開発を始めるとき
- 要件からコードへの落とし込みを学ぶとき
- ポートフォリオ制作の設計を整理したいとき

## Inputs

- 機能説明
- ユーザーストーリー
- 制約条件
- 使用したい技術

## Workflow

1. 要件を機能、データ、制約に分ける。
2. エンティティと関係を抽出する。
3. 必要な画面、API、関数を洗い出す。
4. 実装順序を作る。
5. 最小実装と拡張機能を分ける。

## Outputs

- `architecture-sketch.md`
- `implementation-plan.md`
- `starter-code.md`

## Implementation Idea

ユーザーの曖昧な作りたいものを、実装可能な小さなタスクへ分解する。

## Example

「読書記録アプリを作りたい」という要件から、Bookモデル、登録API、一覧画面、検索機能、実装順序を作る。

## Future Improvements

- ER図の自動生成
- Starter codeの生成
- 受け入れ条件との連携
