# Design Pattern Detective

## Metadata

| Field | Value |
|---|---|
| Category | Learning |
| Difficulty | Beginner |
| Estimated time | 20-45 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Source code, class/module structure |
| Tags | learning, design-pattern, oop, code-reading |

## Purpose

既存コードから設計パターンを発見し、実コードの中でどのように使われているか学ぶ。

## Use Cases

- オブジェクト指向設計の学習
- OSS読解
- Strategy、Factory、Observer、Adapterなどの理解

## Inputs

- ソースコード
- ディレクトリ構成
- 学びたい設計パターン

## Workflow

1. クラスやモジュールの関係を抽出する。
2. パターン候補を検出する。
3. その設計が選ばれた理由を説明する。
4. 利点と欠点を整理する。
5. 代替設計と練習課題を提示する。

## Outputs

- `pattern-report.md`
- `architecture-diagram.md`
- `exercises.md`

## Implementation Idea

コードベースを読ませ、構造上の特徴から設計パターンを推測し、初心者向けの説明に変換する。

## Example

決済処理の実装から Strategy Pattern を検出し、支払い方法追加時に変更箇所が少なくなる理由を説明する。

## Future Improvements

- クラス図生成
- パターン検出精度の改善
- アンチパターン検出との連携
