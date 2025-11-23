# 実験ガイド

このドキュメントでは、Claude Codeの挙動を体系的に実験する方法を説明します。

## 実験の目的

Claude Codeの機能について、実際の利用シーンでの挙動を検証し、最適な使い方を見つけることが目的です。

## 実験の種類

### 挙動検証

特定の機能の動作を確認する実験
- サブエージェントの出力伝達
- スキルのコンテキスト共有
- コマンドの実行結果

**テンプレート**: [basic-experiment](../templates/basic-experiment/)

### 比較実験

複数のアプローチを比較する実験
- サブエージェント vs スキル vs メイン
- 異なる条件での効果比較

**テンプレート**: [comparison-experiment](../templates/comparison-experiment/)

### 効果測定

機能の効果を定量的に評価する実験
- 所要時間の比較
- トークン使用量の測定
- 成果物品質の評価

### 再現性確認

過去の観察を再検証する実験
- 報告された挙動の確認
- バージョンアップ後の変化検証

## 実験の進め方

### 1. テンプレートの選択

[templates/](../templates/) から適切なテンプレートを選択します。

### 2. リポジトリの作成

新しいリポジトリを作成し、テンプレートをコピーします。

```bash
# 例: 実験02の場合
git clone git@github.com:trust-delta/claude-code-experiments.git
cd claude-code-experiments
cp -r templates/basic-experiment ../claude-code-exp02-your-topic
cd ../claude-code-exp02-your-topic
git init
```

### 3. 実験の実施

テンプレートのREADME.mdに従って実験を実施します。

### 4. 結果の記録

- 実行ログを詳細に記録
- スクリーンショットを保存
- 観察や気づきをメモ

### 5. 知見の整理

実験から得られた知見を明確化します：
- ベストプラクティス
- アンチパターン
- 適用シーン

### 6. 成果の共有

umbrella リポジトリのREADME.mdに実験情報を追加します。

## 実験リポジトリの命名規則

```
claude-code-expXX-{topic-name}
```

- `XX`: 実験番号（01, 02, 03...）
- `{topic-name}`: 実験テーマをケバブケースで記述

例：
- `claude-code-exp01-subagent-output`
- `claude-code-exp02-subagent-dialog`
- `claude-code-exp03-skill-context`

## ヒント

### 記録について

- **詳細に**: 後から振り返りやすいよう、詳しく記録
- **客観的に**: 主観だけでなく、具体的な事実を記録
- **タイムスタンプ**: いつ何が起きたか分かるように

### 実験設計について

- **明確な目的**: 何を明らかにしたいか明確に
- **仮説を立てる**: 予想を記述しておく
- **比較可能に**: 条件を揃えて公平に比較

### 知見の抽出について

- **具体的に**: 抽象的でなく具体的に記述
- **再現可能に**: 他の人が同じことを試せるように
- **実践的に**: すぐに使える形で整理

## 参考資料

- [分析ガイド](analysis-guide.md)
- [Claude Code 公式ドキュメント](https://docs.anthropic.com/en/docs/agents/claude-code)
