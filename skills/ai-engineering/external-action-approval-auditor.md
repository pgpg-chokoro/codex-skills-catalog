# External Action Approval Auditor

## Metadata

| Field | Value |
|---|---|
| Category | AI Engineering |
| Difficulty | Intermediate |
| Estimated time | 30-45 min |
| Useful for | Codex / OpenClaw / Claude Code / Gemini CLI / Cursor |
| Required tools | Skill docs, action logs, approval UI, dry-run output |
| Tags | ai-engineering, agent, approval, external-actions, safety, testing |

## Purpose

外部アカウント、公開投稿、課金対象APIなど、実世界に影響するエージェント操作について、実行前のプレビュー、明示承認、資格情報の扱い、停止条件を監査する。

## Use Cases

- X/Twitter、Slack、GitHub、メールなどに投稿する Skill を公開前に確認したいとき
- TweetClaw のような OpenClaw plugin を使う Skill で、投稿前承認と失敗時の停止条件を明文化したいとき
- 読み取り専用操作と、公開・非公開・課金対象の操作を分けたいとき
- 資格情報やアカウント識別子がログ、fixture、プロンプトへ漏れないか確認したいとき

## Inputs

- Skill の `SKILL.md`
- README または利用手順
- ツール一覧と権限一覧
- プレビューまたは dry-run の出力例
- 失敗時のエラー例

## Workflow

1. Skill が呼び出す外部アクションをすべて列挙する。
2. 各アクションを読み取り専用、公開操作、非公開操作、課金対象操作、定期実行に分類する。
3. 書き込み系アクションで、実行前に対象アカウント、送信本文、添付、実行範囲をプレビューできるか確認する。
4. 公開操作、非公開操作、課金対象操作、定期実行では、明示承認なしに実行されないことを確認する。
5. 資格情報、Cookie、セッション、APIキーがプロンプト、ログ、fixture、エラー出力に保存されないことを確認する。
6. rate limit、認証失敗、権限不足、プラットフォーム制限などの停止条件を確認する。
7. 不足している承認、プレビュー、ログ削除、テスト観点を修正候補としてまとめる。

## Outputs

- `approval-audit.md`
- `action-safety-matrix.md`
- `regression-checklist.md`

## Implementation Idea

`SKILL.md` として実装する場合は、外部ツール定義、approval hook、README、テスト fixture を読み、アクションごとに「分類」「プレビュー」「承認」「資格情報」「停止条件」を表で出力する。TweetClaw などの X/Twitter Skill では、投稿本文の完全なプレビューとユーザー承認を必須チェックにする。

## Example

TweetClaw を使う X/Twitter 投稿 Skill を監査する場合、投稿本文、返信先、メディア、対象アカウントをプレビューし、承認後にだけ実行されることを確認する。認証失敗や rate limit では再試行ではなく停止し、利用者に次の操作を提示する。

## Future Improvements

- approval hook の自動テスト生成
- 既存ログからの資格情報漏えいパターン検出
- 外部アクションごとの回帰テストテンプレート生成
