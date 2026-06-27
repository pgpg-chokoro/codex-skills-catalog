# Refactor Playground Builder

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Programming language, learning goal |
| Tags | learning, refactoring, code-review, beginner |

## Purpose

わざと改善余地のあるコードを生成し、段階的なリファクタリング練習環境を作る。

## Use Cases

- リファクタリング演習
- コードレビュー練習
- オブジェクト指向や関数分割の学習

## Inputs

- 学習したい言語
- 題材となる小さなアプリ
- 学習者のレベル

## Workflow

1. 教材用の問題コードを生成する。
2. 改善点を列挙する。
3. 段階的なリファクタリング課題に分ける。
4. ヒントを作る。
5. 模範解答と解説を作る。

## Outputs

- `starter-code/`
- `refactor-tasks.md`
- `solution-walkthrough.md`

## Implementation Idea

長すぎる関数、重複コード、曖昧な命名、密結合を含む教材コードを作り、改善順序を学べるようにする。

## Example

TODOアプリの処理を1つの巨大関数にまとめたコードから、入力処理、保存処理、表示処理を分割する演習を作る。

## Future Improvements

- 難易度別教材生成
- テスト付き演習
- Before / After 比較レポート
