# Library Source Tour Guide

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Intermediate |
| Estimated time | 30-90 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Repository, learner level |
| Tags | learning, oss, code-reading, library |

## Purpose

ライブラリの内部構造を段階的に読むための案内を作る。

## Use Cases

- OSSの中身を読みたいとき
- 公開APIの裏側を理解したいとき
- 既存ライブラリの設計を学びたいとき

## Inputs

- 対象リポジトリ
- 学習者のレベル
- 理解したい機能

## Workflow

1. 公開APIと入口となるファイルを探す。
2. 主要モジュールを整理する。
3. 代表的な処理の流れを追う。
4. 読む順番を作る。
5. 発展的に読むべき箇所を示す。

## Outputs

- `reading-route.md`
- `architecture-overview.md`
- `advanced-topics.md`

## Implementation Idea

巨大なライブラリを一度に読ませず、小さな探索ルートへ分解する。

## Example

Webライブラリのリクエスト処理を、入口、ルーティング、処理本体、レスポンス生成の順に読む。

## Future Improvements

- バージョン別読解ガイド
- 実行ログとの連携
- 読解課題の自動生成
