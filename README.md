# Codex Skills Catalog

Codex / AI Coding Agent 向けの再利用可能な Skill を収集・整理する公開カタログです。

このリポジトリでは、単発のプロンプトではなく、**入力・手順・成果物を持つ再利用可能な作業ワークフロー**として Skill を整理します。

## 目的

- AIエンジニア実務向け Skill の蓄積
- 開発初学者向け学習 Skill の蓄積
- 面白い・実験的な Skill の発掘
- 重複紹介の抑制
- Codex / Claude Code / Gemini CLI / Cursor などで再利用しやすい形への整理

## カテゴリ

| Category | Description |
|---|---|
| AI Engineering | LLM / RAG / Agent / 評価 / 実験管理など、AIエンジニアリング実務向け |
| DevOps | 障害対応、リリース、依存関係、ナレッジ運用など |
| Learning | 初学者が開発力を伸ばすための教材化・読解支援 |
| Architecture | 設計判断、トレードオフ、システム理解 |
| Fun | 勉強会・発想支援・創作的分析に向いた実験的 Skill |

## ディレクトリ構成

```text
.
├── README.md
├── POLICY.md
├── CATALOG.md
├── docs/
│   ├── categories.md
│   └── contribution.md
├── index/
│   ├── categories.md
│   └── introduced-skills.md
├── skills/
│   ├── ai-engineering/
│   ├── architecture/
│   ├── devops/
│   ├── fun/
│   └── learning/
└── templates/
    └── SKILL_TEMPLATE.md
```

## Skill の読み方

各 Skill は、以下の観点で整理しています。

- **Purpose**: 何をする Skill か
- **Use Cases**: いつ使うか
- **Inputs**: 必要な入力
- **Workflow**: エージェントに実行させる手順
- **Outputs**: 期待する成果物
- **Implementation Idea**: `SKILL.md` 化する際の実装案
- **Tags**: 検索用タグ

## 主要 Skill

- [AI Experiment Ledger](skills/ai-engineering/ai-experiment-ledger.md)
- [Prompt Contract Enforcer](skills/ai-engineering/prompt-contract-enforcer.md)
- [Context Window Budget Manager](skills/ai-engineering/context-window-budget-manager.md)
- [Dependency Upgrade Navigator](skills/devops/dependency-upgrade-navigator.md)
- [Library Source Tour Guide](skills/learning/library-source-tour-guide.md)
- [Design Tradeoff Studio](skills/architecture/design-tradeoff-studio.md)
- [Framework Fusion Lab](skills/fun/framework-fusion-lab.md)

一覧は [CATALOG.md](CATALOG.md) を参照してください。

## 追加方針

1. 既存 Skill と同じカテゴリ・同じワークフローファミリーでないか確認する。
2. 近い Skill がある場合は、別 Skill として増やすより統合を優先する。
3. `templates/SKILL_TEMPLATE.md` に沿って書く。
4. 個人情報、企業内部情報、認証情報、会話履歴は保存しない。

## 公開ポリシー

このリポジトリには、個人情報、企業内部情報、非公開研究内容、認証情報、会話履歴を保存しません。

詳細は [POLICY.md](POLICY.md) を参照してください。
