# API Explorer Tutor

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 20-45 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | API documentation, OpenAPI spec, sample credentials if available |
| Tags | learning, api, backend, beginner |

## Purpose

初めて触るAPIを、初心者が学びやすい教材と演習へ変換する。

## Use Cases

- REST APIやSaaS APIを学び始めるとき
- APIドキュメントの読み方を学びたいとき
- 小さなサンプルアプリを作りたいとき

## Inputs

- API仕様
- 学習者のレベル
- 作りたい小さな成果物

## Workflow

1. API仕様を読み、重要なエンドポイントを抽出する。
2. 最初に覚えるべき概念を整理する。
3. 学習順序を作る。
4. サンプルリクエストを生成する。
5. 演習課題と理解度チェックを作る。

## Outputs

- `learning-path.md`
- `example-requests.md`
- `exercises.md`

## Implementation Idea

APIドキュメントを入力し、認証、取得、作成、更新、削除の基本操作を小さな課題に分解する。

## Example

GitHub APIを題材に、リポジトリ一覧取得、Issue作成、検索API利用を段階的に学ぶ。

## Future Improvements

- OpenAPIからの自動教材化
- Postman / curl / Python サンプル生成
- エラー時のデバッグガイド生成
