# 📦 claude-kit

このリポジトリは Claude Code を安全に活用するためのテンプレート集です。  
AIアシスタントと安心して共同作業するために、**禁止事項・確認ルール・起動テンプレ**を整備しています。

---

## 🔧 構成ファイル

| ファイル名 | 目的 |
|------------|------|
| `.claude/settings.json` | 危険なコマンド・外部通信・機密アクセスのブロック設定 |
| `SECURITY.md` | Claudeに守らせる禁止ルールと行動ガイド |
| `Claude起動テンプレ.md` | Claude Code起動時に渡すテンプレート |
| `Claudeプロンプト集.md` | よく使う指示やテンプレ文をまとめたもの |
| `Claude設定メモ.md` | `.claude/settings.json` の中身をMarkdownで管理（編集用） |

---

## ✅ Claude起動時の使い方

1. `.claude/settings.json` をプロジェクトに配置する
2. Claudeに「`SECURITY.md` を読んでから作業して」と指示
3. `Claude起動テンプレ.md` の内容を毎回提示する
4. すべての操作で「Yes/No確認 → 実行」のプロセスを守る

---

## 📌 利用例（Claudeに渡す指示例）

このプロジェクトは claude-kit に準拠しています。

以下のファイルを読み込んでから作業を開始してください：

---

## 🔐 注意

- このテンプレは誰でも使えますが、**APIキーや個人情報は絶対に含めないでください**。
- 公開用に使用する場合は `.env` や秘密鍵ファイルは含めないよう注意してください。

---

## 📜 ライセンス

MIT License

- .claude/settings.json
- SECURITY.md
- Claude起動テンプレ.md