# Prompt Contract Enforcer

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Intermediate |
| Estimated time | 20-40 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Prompt set, schema validator, test cases |
| Tags | ai-engineering, llm, prompt, structured-output, testing |

## Purpose

LLMアプリケーションにおける「このプロンプトはこの形式の出力を返す」という契約を定義・検証する。

## Use Cases

- Structured Output を安定運用したいとき
- モデル更新後の出力崩れを検出したいとき
- エージェントのツール呼び出し条件をテストしたいとき

## Inputs

- 対象プロンプト
- 出力スキーマ
- 禁止表現や必須フィールド
- テストケース

## Workflow

1. プロンプトごとの出力契約を定義する。
2. 基準テストケースを実行する。
3. JSON Schema などで構造を検証する。
4. 契約違反を分類する。
5. 修正案と再テスト手順を出力する。

## Outputs

- `contract-report.md`
- `schema-violations.md`
- `prompt-fixes.md`

## Implementation Idea

CIで定期的にプロンプトテストを実行し、出力形式、必須フィールド、禁止表現、ツール呼び出しの期待条件を検証する。

## Example

問い合わせ分類プロンプトが必ず `{category, confidence, reason}` を返すか確認し、欠落や余計な文章を検出する。

## Future Improvements

- CI連携
- スキーマ差分の自動レビュー
- モデル別の契約遵守率比較
