# Claude Code Experiments

Claude Codeの挙動を体系的に実験・検証するリポジトリです。

## 使い方

各実験ディレクトリをIDEで開いてClaude Codeを使用してください。

```bash
cd exp01-subagent-context-isolation
code .  # IDEで開く
```

## 実験一覧

| ID | タイトル | ディレクトリ | 実験日 | ステータス |
|----|---------|------------|--------|-----------|
| 01 | サブエージェントのコンテキスト分離レベルの確認 | [exp01-subagent-context-isolation/](./exp01-subagent-context-isolation/) | 2025-11-21 | ✅ 完了 |
| 02 | 対話的タスクにおけるサブエージェントの挙動 | [exp02-subagent-dialog/](./exp02-subagent-dialog/) | 2025-11-28 | ✅ 完了 |

## ドキュメント

- [実験ガイド](docs/experiment-guide.md)
- [分析ガイド](docs/analysis-guide.md)

## 新しい実験を追加

1. 新しいディレクトリを作成（例: exp03-xxx/）
2. .claude/ディレクトリを配置
3. 実験を実施
4. このREADMEの表を更新
