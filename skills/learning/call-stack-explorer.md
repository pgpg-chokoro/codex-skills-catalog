# Call Stack Explorer

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 15-35 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Source code, sample input |
| Tags | learning, debugging, execution-flow |

## Purpose

関数がどの順番で呼ばれ、どの順番で戻るかを可視化して、プログラムの実行の流れを学ぶ。

## Use Cases

- 関数呼び出しの流れを理解したいとき
- 再帰や例外処理を学ぶとき
- デバッグの基礎を身につけたいとき

## Inputs

- ソースコード
- サンプル入力
- 注目したい関数

## Workflow

1. 実行開始点を特定する。
2. 呼び出される関数を順番に並べる。
3. 各関数の入力と戻り値を記録する。
4. 実行の流れを図や表にする。
5. 理解確認用の小問を作る。

## Outputs

- `execution-trace.md`
- `call-graph.md`
- `learning-notes.md`

## Implementation Idea

小さな入力例を使い、関数呼び出しと戻り値の流れを時系列で説明する。

## Example

再帰関数の例で、深く呼び出されてから順に戻っていく流れを説明する。

## Future Improvements

- Mermaid図の生成
- デバッガ操作ガイドとの連携
- 実行ログからの自動トレース
