# Specification Detective

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 20-40 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Requirements, feature requests |
| Tags | learning, specification, requirements, planning |

## Purpose

仕様書や要件書を読み解き、実際に何を作ればよいのかを整理する。

## Use Cases

- チーム開発入門
- ハッカソンや開発演習
- 曖昧な要求を実装可能な形にしたいとき

## Inputs

- 仕様書
- 機能要望
- 関連する制約や前提

## Workflow

1. 要求を抽出する。
2. 用語を整理する。
3. 曖昧な点と未決事項を特定する。
4. ユースケースを作る。
5. 受け入れ条件を作る。

## Outputs

- `clarified-spec.md`
- `use-cases.md`
- `acceptance-criteria.md`

## Implementation Idea

実装前に仕様を構造化し、何を作るべきか、何を確認すべきか、何を完了条件とするかを明確にする。

## Example

「ユーザーが投稿を管理できる」という要望から、作成、編集、削除、一覧、権限、エラー時の挙動を整理する。

## Future Improvements

- Requirement-to-Code Translatorとの連携
- テストケース生成
- 仕様レビュー用チェックリスト
