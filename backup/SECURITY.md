# 🔒 Claude セキュリティルール

Claude はこのルールを常に守って行動してください。  
以下の操作は一切禁止とし、提案・実行・補助も行わないこと。

---

## ❌ 禁止されている操作

### 🧨 危険コマンド
- `sudo`, `rm`, `rm -rf`, `dd`, `mkfs`, `:(){ :|:& };:`
- `chmod 777` などの無制限権限コマンド

### 🌐 外部通信
- `curl`, `wget`, `nc` などによる外部アクセス
- `curl | sh` など外部スクリプトの実行

### 🔏 機密ファイルアクセス
- `.env`, `id_rsa`, `id_ed25519`, `*.pem`, `*token*`, `*key*`, `secrets/**`
- 上記の読み取り／書き込み／表示

### 🛠️ Git／パッケージ操作
- `git push`, `git commit`, `git reset`, `git rebase`
- `npm uninstall`, `npm remove` など依存性の削除操作

### 🛢️ データベース関連
- `psql`, `mysql`, `mongod` などへの直接接続
- `DROP`, `DELETE FROM`, `TRUNCATE` を含むSQL命令
- `mcp__supabase__execute_sql` などClaude経由でのDB操作

---

## 📘 Claudeへの行動ルール

1. 作業を始める前に **.claude/settings.json** とこの `SECURITY.md` を読んでください。
2. 危険・禁止項目に該当する内容は、**提案・実行しないでください**。
3. 判断に迷う操作は、必ず「保留」し人間に確認してください。
4. すべての操作は **Yes/No確認をとってから** 実行してください。

---

このルールは Claude Code 環境で安全に共同作業を行うための基本原則です。