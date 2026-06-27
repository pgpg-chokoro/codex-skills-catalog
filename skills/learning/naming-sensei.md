# Naming Sensei

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 10-25 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Source code, domain context |
| Tags | learning, naming, readability, refactoring |

## Purpose

変数名、関数名、クラス名の付け方を学び、コードの可読性を高める。

## Use Cases

- `data`、`tmp`、`value` のような曖昧な名前を改善したいとき
- コードレビューで命名観点を学びたいとき
- ドメイン知識を反映した名前を考えたいとき

## Inputs

- 対象コード
- ドメイン説明
- 命名ルール

## Workflow

1. 曖昧な識別子を抽出する。
2. 各識別子の役割を分析する。
3. ドメイン語彙を抽出する。
4. 命名候補を複数出す。
5. 改善理由を説明する。

## Outputs

- `naming-review.md`
- `rename-suggestions.md`
- `naming-guidelines.md`

## Implementation Idea

コードを読んで変数や関数の役割を推測し、意図が伝わる名前へ変換する。

## Example

`data` を `activeUsers`、`calculate` を `calculateMonthlyRevenue` のように、役割が分かる名前へ改善する。

## Future Improvements

- プロジェクト命名規則の自動抽出
- rename用パッチ生成
- ドメイン用語集との連携
