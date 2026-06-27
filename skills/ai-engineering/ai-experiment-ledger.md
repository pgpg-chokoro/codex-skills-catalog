# AI Experiment Ledger

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Intermediate |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Git, experiment logs, evaluation outputs |
| Tags | ai-engineering, llm, evaluation, reproducibility |

## Purpose

LLM、RAG、AI Agent 開発で行った実験を、再現可能な実験台帳として整理する。

## Use Cases

- プロンプト改善の履歴を残したいとき
- モデル比較の条件を後から追えるようにしたいとき
- 失敗実験を次の改善材料として蓄積したいとき

## Inputs

- 実験目的
- 使用モデル、プロンプト、ツール、データセット
- 評価指標と実行結果
- 失敗例や観察メモ

## Workflow

1. 実験の仮説と目的を整理する。
2. 実験条件を表形式で記録する。
3. 入力、出力、評価指標を紐づける。
4. 成功・失敗要因を分類する。
5. 次に試すべき改善案を生成する。

## Outputs

- `experiment-log.md`
- `comparison-table.md`
- `next-actions.md`

## Implementation Idea

AI実験を実行した直後にこの Skill を呼び出し、設定ファイル、評価結果、代表的な失敗出力を読み取って Markdown 台帳へ変換する。

## Example

RAGの検索件数を `top_k=3` から `top_k=8` に変えた実験について、回答品質、レイテンシ、失敗例を比較表に残す。

## Future Improvements

- Weights & Biases や MLflow との連携
- Git commit と実験IDの自動紐づけ
- 失敗タイプ別の自動タグ付け
