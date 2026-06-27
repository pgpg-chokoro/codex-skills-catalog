# Test Case Inventor

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 20-45 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Source code, feature description |
| Tags | learning, testing, qa, beginner |

## Purpose

完成したコードや仕様に対して、どんなテストを書くべきかを考える力を育てる。

## Use Cases

- 単体テスト学習
- QA入門
- TDD前のテスト観点整理
- コードレビュー練習

## Inputs

- 対象コード
- 機能説明
- 入力値の制約
- 期待される振る舞い

## Workflow

1. 入力と出力を整理する。
2. 正常系を列挙する。
3. 境界値を抽出する。
4. 異常系と例外ケースを考える。
5. テストマトリクスを作る。

## Outputs

- `test-matrix.md`
- `edge-cases.md`
- `practice-tests.md`

## Implementation Idea

正常系だけでなく、空値、境界値、異常入力、同時実行、タイムゾーンなどの観点を体系的に提示する。

## Example

日付入力機能に対し、空文字、未来日、うるう日、タイムゾーン差、フォーマット不正のケースを生成する。

## Future Improvements

- テストコード自動生成
- カバレッジ不足の検出
- 仕様書からのテスト観点抽出
