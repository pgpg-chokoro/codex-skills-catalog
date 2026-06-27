# Design Tradeoff Studio

## Metadata

| Field | Value |
|---|---|
| Category | Architecture |
| Difficulty | Beginner |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Requirements, constraints |
| Tags | architecture, design, tradeoff, learning |

## Purpose

複数の設計案を比較し、制約に応じて判断する力を養う。

## Use Cases

- システム設計入門
- 個人開発の技術選定
- 技術面接対策
- 設計レビューの練習

## Inputs

- 機能要件
- 非機能要件
- 制約条件
- 比較したい技術や設計案

## Workflow

1. 設計案を複数作る。
2. 評価軸を定義する。
3. 各案の利点と欠点を比較する。
4. 制約に対する適合度を評価する。
5. 推奨案と採用理由をまとめる。

## Outputs

- `design-options.md`
- `tradeoff-table.md`
- `recommendation.md`

## Implementation Idea

唯一の正解を探すのではなく、制約の中でどの設計が妥当かを比較表で学べるようにする。

## Example

メモアプリを、ローカル保存、DB保存、クラウド同期の3案で比較し、目的に応じた選択理由を整理する。

## Future Improvements

- ADR形式への変換
- コスト見積もりの追加
- Technology Futures Labとの連携
