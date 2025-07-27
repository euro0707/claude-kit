# 📦 claude-kit

このリポジトリは Claude Code を安全かつ快適に活用するためのスターターテンプレート集です。  
AIアシスタントと安心して共同作業するために、**禁止事項・確認ルール・起動テンプレ**を整備しています。

---

## 🔧 構成ファイル

| ファイル名            | 目的 |
|-----------------------|------|
| `.claude/settings.json` | 危険なコマンド・外部通信・機密アクセスのブロック設定＋初期ファイル自動生成設定 |
| `SECURITY.md`          | Claudeに守らせる禁止ルールと行動ガイド |
| `StartupTemplate.md`   | Claude Code起動時に渡すテンプレート |
| `ClaudePrompt.md`      | よく使う指示やテンプレ文をまとめたもの |
| `Claude設定メモ.md`     | `.claude/settings.json` の中身をMarkdownで管理（編集用）※任意 |

---

## ✅ Claude Code 起動時の使い方

1. Claude Code でプロジェクトを作成  
2. `.claude/settings.json` を読み込む（初期設定＆ファイル生成）  
3. Claudeに「まず `SECURITY.md` を読んで」と指示  
4. `StartupTemplate.md` をそのまま貼る or 自動提示  
5. すべての操作で「Yes/No確認 → 実行」のルールを守る

---

## 📌 Claudeに渡す例

```
このプロジェクトでは claude-kit に準拠します。
以下の3ファイルを読んでから作業してください：

- SECURITY.md
- StartupTemplate.md
- ClaudePrompt.md
```

---

## 🔐 注意

- このテンプレは誰でも使えますが、**APIキーや個人情報は含めないでください**
- `.env`や秘密鍵ファイルは絶対にアップロードしないこと
- Claude Codeの挙動はモデルにより変わるため注意深く使ってください

---

## 📜 ライセンス

MIT License
