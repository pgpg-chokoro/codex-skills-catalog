# Contribution Guide

このリポジトリでは、Codex / AI Coding Agent で再利用しやすい Skill を整理する。

## 基本方針

- 単なるアイデアではなく、実行手順と成果物を持つ Skill として書く。
- 既存 Skill と重複する場合は、新規追加より統合を優先する。
- 公開リポジトリに置ける一般化された内容だけを書く。
- 個人情報、企業内部情報、認証情報、非公開研究内容、会話履歴は含めない。

## 追加手順

1. `CATALOG.md` で既存 Skill を確認する。
2. 近い Skill があれば、その Skill の `Future Improvements` に追加する。
3. 新規 Skill の場合は、適切なカテゴリ配下に Markdown ファイルを作る。
4. `templates/SKILL_TEMPLATE.md` に沿って内容を書く。
5. `CATALOG.md` と `index/introduced-skills.md` に追記する。

## 命名ルール

- ファイル名は kebab-case にする。
- Skill 名は Title Case にする。
- ワークフローファミリーが分かる名前にする。

例:

```text
skills/ai-engineering/prompt-contract-enforcer.md
skills/learning/call-stack-explorer.md
skills/fun/framework-fusion-lab.md
```

## 推奨タグ

- `ai-engineering`
- `llm`
- `agent`
- `rag`
- `evaluation`
- `devops`
- `testing`
- `debugging`
- `architecture`
- `learning`
- `documentation`
- `fun`
- `creative`

## レビュー観点

- Skill として再利用可能か
- 入力・手順・成果物が明確か
- 既存 Skill と過度に重複していないか
- 公開して問題ない内容か
- 初見の人が使える粒度か
