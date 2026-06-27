# Interface Reverse Engineer

## Metadata

| Field | Value |
|---|---|
| Category | Architecture |
| Difficulty | Intermediate |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Screenshots, behavior notes, optional network logs |
| Tags | architecture, ui, reverse-engineering, learning |

## Purpose

既存アプリやWebサービスの画面から、裏側のデータモデル、API、状態遷移を推測する。

## Use Cases

- Web開発の設計感覚を身につけたいとき
- 既存システムを理解したいとき
- UIからバックエンド構造を想像する訓練をしたいとき

## Inputs

- 画面スクリーンショット
- 操作手順
- 表示されるデータ
- 画面遷移

## Workflow

1. 画面要素を抽出する。
2. 表示データからエンティティを推定する。
3. 必要そうなAPIを仮説化する。
4. 状態遷移を整理する。
5. 仮説アーキテクチャを作る。

## Outputs

- `inferred-architecture.md`
- `api-hypothesis.md`
- `sample-implementation.md`

## Implementation Idea

画面観察から、どんなデータがあり、どんな操作で状態が変わるかを推測する。

## Example

タスク管理画面から、Task、User、Projectモデルと、作成、更新、完了、削除APIを推測する。

## Future Improvements

- ブラウザ開発者ツールログとの連携
- 実装コードとの答え合わせ
- API設計演習への展開
