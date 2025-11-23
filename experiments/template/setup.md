# 実験環境セットアップ

この実験を実施するための環境構築手順を記載します。

## 📋 前提条件

実験を開始する前に以下が準備されていることを確認してください：

- [ ] Claude Code がインストールされている
- [ ] Node.js がインストールされている（推奨バージョン: XX.x以上）
- [ ] Git がインストールされている
- [ ] [その他の必要なツール]

## 🔧 環境構築手順

### 1. プロジェクトのクローン（必要な場合）

```bash
# このリポジトリのルートディレクトリで実行
cd experiments/XX-experiment-name
```

### 2. 依存関係のインストール

```bash
# 必要なパッケージをインストール
npm install

# または
pnpm install
```

### 3. 設定ファイルの準備

[必要な設定ファイルがある場合は記載]

```bash
# 設定ファイルのコピー
cp .env.example .env

# 必要に応じて編集
vim .env
```

### 4. Claude Code の設定

[Claude Code 固有の設定が必要な場合]

#### スキルのインストール（必要な場合）

```bash
# スキルをインストール
[インストールコマンド]
```

#### スラッシュコマンドの設定（必要な場合）

1. `.claude/commands/` ディレクトリを作成
2. コマンドファイルを配置

```bash
mkdir -p .claude/commands
cp [source] .claude/commands/
```

#### MCP サーバーの設定（必要な場合）

`claude_desktop_config.json` に以下を追加：

```json
{
  "mcpServers": {
    "server-name": {
      "command": "node",
      "args": ["path/to/server.js"]
    }
  }
}
```

### 5. 実験用データの準備

[サンプルデータやテストケースの準備]

```bash
# データ生成スクリプトを実行
npm run generate-test-data
```

## ✅ 環境確認

セットアップが正しく完了したか確認します：

```bash
# 確認コマンド1
[コマンド]

# 確認コマンド2
[コマンド]
```

**期待される出力**:
```
[正常な出力の例]
```

## 🎯 実験用のディレクトリ構造

セットアップ完了後、以下の構造になっているはずです：

```
XX-experiment-name/
├── README.md
├── setup.md
├── analysis.md
├── [実験固有のディレクトリ]
│   ├── pattern-a/
│   ├── pattern-b/
│   └── pattern-c/
└── [その他のファイル]
```

## 🔍 トラブルシューティング

### 問題1: [よくある問題]

**症状**:
```
[エラーメッセージ]
```

**解決方法**:
```bash
[解決手順]
```

### 問題2: [よくある問題]

**症状**:
```
[エラーメッセージ]
```

**解決方法**:
```bash
[解決手順]
```

## 📝 環境情報の記録

実験を開始する前に、以下の環境情報を記録してください：

```bash
# システム情報
uname -a

# Claude Code バージョン
claude --version

# Node.js バージョン
node --version

# npm バージョン
npm --version
```

**記録テンプレート**:

```markdown
- 実験実施日: YYYY年MM月DD日
- OS: [OS名とバージョン]
- Claude Code: [バージョン]
- Node.js: [バージョン]
- npm: [バージョン]
- その他: [追加情報]
```

## 🚀 次のステップ

環境構築が完了したら、[README.md](README.md) の実験手順に従って実験を開始してください。
