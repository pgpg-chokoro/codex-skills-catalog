# Evaluation Dataset Curator

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Intermediate |
| Estimated time | 30-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Model outputs, feedback logs, evaluation data |
| Tags | ai-engineering, evaluation, dataset, llm |

## Purpose

LLM・RAG・エージェントの評価データセットを継続的に管理・改善する。

## Use Cases

- 失敗事例を評価ケースとして蓄積したいとき
- 評価データが古くなってきたとき
- モデル改善が本当に品質向上につながっているか確認したいとき

## Inputs

- モデル出力
- 失敗事例
- ユーザーフィードバック
- 既存評価データ

## Workflow

1. 失敗事例を抽出する。
2. 失敗タイプを分類する。
3. 重複を除去する。
4. 難易度と重要度を付ける。
5. 評価データセットへ追加する。
6. カバレッジを確認する。

## Outputs

- `eval-dataset.jsonl`
- `coverage-report.md`
- `failure-taxonomy.md`

## Implementation Idea

日々の運用ログやレビュー結果から、代表的な失敗を評価ケースへ変換し、回帰テストに追加する。

## Example

RAGで根拠文書があるのに回答が曖昧になったケースを抽出し、「根拠利用不足」カテゴリとして評価データに加える。

## Future Improvements

- 自動重複判定
- 失敗タイプ別のサンプリング
- 評価ケースの劣化検出
