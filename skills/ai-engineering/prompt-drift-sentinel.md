# Prompt Drift Sentinel

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Intermediate |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Baseline outputs, evaluation cases, model config |
| Tags | ai-engineering, llm, monitoring, regression-test |

## Purpose

プロンプト、モデル、ツール、システム指示の変更によるAIシステムの品質劣化を検出する。

## Use Cases

- RAGやAIエージェントを継続運用しているとき
- モデルやプロンプトを変更したとき
- 回答品質、ツール利用率、レイテンシの変化を追いたいとき

## Inputs

- 基準評価ケース
- 現在のプロンプトとモデル設定
- 過去の評価結果
- 期待する品質基準

## Workflow

1. 基準ケースを現在の構成で実行する。
2. 過去結果と比較する。
3. 差分を品質、形式、ツール利用、速度に分類する。
4. 劣化がある場合は原因候補を挙げる。
5. 回復案と追加テストを提案する。

## Outputs

- `drift-report.md`
- `regression-summary.md`
- `mitigation-plan.md`

## Implementation Idea

モデル更新やプロンプト変更のたびに、固定の評価セットを実行し、出力差分を自動分類する。

## Example

FAQ Botのモデル更新後に、回答根拠の引用率が下がっていないか、拒否すべき質問に答えていないかを確認する。

## Future Improvements

- 差分の自動重大度判定
- 品質メトリクスの時系列可視化
- Prompt Contract Enforcer との連携
