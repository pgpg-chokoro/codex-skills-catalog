# Bug Cryptozoologist

## Metadata

| Field | Value |
|---|---|
| Category | Fun |
| Difficulty | Intermediate |
| Estimated time | 20-60 min |
| Useful for | Codex / Claude Code / Gemini CLI / Cursor |
| Required tools | Repository, issue history, architecture notes |
| Tags | fun, bug, edge-case, code-review |

## Purpose

まだ発見されていない奇妙な不具合を、遊び感覚で推理する。

## Use Cases

- コードレビューイベント
- 勉強会
- エッジケース探索
- 品質意識のトレーニング

## Inputs

- 対象リポジトリ
- 既知のIssue
- アーキテクチャ概要
- 重要な入力条件

## Workflow

1. 危険そうな領域を探す。
2. まれな条件を列挙する。
3. 起こり得る不具合の仮説を作る。
4. 再現シナリオを考える。
5. リスク観察メモを作る。

## Outputs

- `hypothetical-bugs.md`
- `reproduction-scenarios.md`
- `risk-observations.md`

## Implementation Idea

タイムゾーン、特殊文字、キャッシュ、並行処理など、通常レビューで漏れがちな条件を楽しく探す。

## Example

うるう日、年末年始、極端に長い入力などで集計処理が崩れないかを仮説化する。

## Future Improvements

- Test Case Inventorとの連携
- 実際のIssueとの照合
- リスク別の優先度付け
