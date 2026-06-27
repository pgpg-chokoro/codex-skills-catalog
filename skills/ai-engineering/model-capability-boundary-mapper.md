# Model Capability Boundary Mapper

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Advanced |
| Estimated time | 45-90 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Evaluation suite, task definitions, metrics |
| Tags | ai-engineering, llm, evaluation, capability, agent |

## Purpose

AIモデルやエージェントが「どこまでできて、どこから失敗し始めるのか」を体系的に測定する。

## Use Cases

- 新モデルの採用可否を判断するとき
- エージェントに任せられるタスク範囲を決めるとき
- コンテキスト長、ステップ数、ツール依存度の限界を知りたいとき

## Inputs

- 対象モデルまたはエージェント
- タスクセット
- 難易度パラメータ
- 評価基準

## Workflow

1. 評価対象タスクを分解する。
2. 難易度を変化させるパラメータを定義する。
3. 段階的に評価を実行する。
4. 失敗が増える境界条件を特定する。
5. 安全な適用範囲をまとめる。

## Outputs

- `capability-map.md`
- `failure-boundaries.md`
- `deployment-guidelines.md`

## Implementation Idea

同じタスクを、入力長、手順数、曖昧さ、ツール利用数を変えながら実行し、成功率が崩れる条件を記録する。

## Example

コード修正エージェントについて、1ファイル修正、複数ファイル修正、仕様変更込み修正の順に難易度を上げて評価する。

## Future Improvements

- 難易度生成の自動化
- モデル間比較レポート
- 本番適用ルールとの連携
