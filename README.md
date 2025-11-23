# Claude Code Experiments

Claude Codeの各機能（サブエージェント、スキル、カスタムスラッシュコマンド）の挙動を体系的に実験・検証し、知見を蓄積するモノレポジトリ。

**作成日**: 2025年11月24日

## 📋 プロジェクト概要

このリポジトリは、Claude Codeの以下の機能について実験・検証を行うことを目的としています：

- **サブエージェント**: 独立したコンテキストでのタスク実行
- **スキル**: 再利用可能な機能モジュール
- **カスタムスラッシュコマンド**: ユーザー定義のコマンド
- **MCP (Model Context Protocol)**: 外部ツールとの統合

## 🧪 実験一覧

| ID | 実験名 | ステータス | 作成日 | 概要 |
|----|--------|-----------|--------|------|
| 01 | サブエージェントの対話的タスク挙動検証 | 準備中 | 2025-11-24 | サブエージェントが対話的タスク（要件定義）に適しているか検証 |

## 📁 リポジトリ構造

```
claude-code-experiments/
├── README.md                 # このファイル
├── experiments/              # 実験ディレクトリ
│   ├── README.md            # 実験インデックス
│   ├── template/            # 実験テンプレート
│   └── 01-*/                # 個別実験
├── docs/                    # ドキュメント
└── .gitignore
```

## 🔄 バージョン管理方針

- **main ブランチ**: 安定した実験結果のみをマージ
- **experiment/* ブランチ**: 個別実験用のブランチ
- **コミットメッセージ**: `[EXP-XX] 説明` の形式（例: `[EXP-01] Add initial setup`）

### コミットプレフィックス

- `[EXP-XX]`: 実験関連
- `[DOC]`: ドキュメント更新
- `[FIX]`: バグ修正
- `[REFACTOR]`: リファクタリング

## 🤝 コントリビューション方法

1. **新しい実験を追加する**:
   ```bash
   # テンプレートをコピー
   cp -r experiments/template experiments/XX-your-experiment-name

   # README.mdを編集して実験内容を記載
   ```

2. **実験を実行する**:
   - 各実験の `setup.md` に従って環境を構築
   - 実験を実行し、結果を `analysis.md` に記録

3. **結果を共有する**:
   - ブランチを作成: `git checkout -b experiment/XX-your-experiment`
   - コミット: `git commit -m "[EXP-XX] Add experiment results"`
   - プルリクエストを作成（該当する場合）

## 📚 参考資料

- [Claude Code 公式ドキュメント](https://docs.anthropic.com/en/docs/agents/claude-code)
- [実験ガイド](docs/experiment-guide.md)
- [実験インデックス](experiments/README.md)

## 📝 ライセンス

このリポジトリは実験・学習目的で作成されています。

## 🔗 関連リンク

- [Claude Agent SDK](https://github.com/anthropics/anthropic-quickstarts/tree/main/claude-agent-sdk)
- [MCP Servers](https://github.com/modelcontextprotocol/servers)
