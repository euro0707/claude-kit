# ⚙️ Claude設定メモ（settings.json）

以下は Claude Code の `.claude/settings.json` に使うべき設定ファイルです。  
PCが使えるようになったら、そのままコピペして `.json` ファイルとして保存できます。

```json
{
  "permissions": {
    "allow": [],
    "deny": [
      "Bash(sudo:*)",
      "Bash(rm:*)",
      "Bash(rm -rf:*)",
      "Bash(dd:*)",
      "Bash(mkfs:*)",
      "Bash(:(){ :|:& };:)",
      "Bash(chmod 777:*)",
      "Bash(curl:*)",
      "Bash(wget:*)",
      "Bash(nc:*)",
      "NetConnect(*)",
      "Read(.env*)",
      "Read(id_rsa)",
      "Read(id_ed25519)",
      "Read(**/*token*)",
      "Read(**/*key*)",
      "Read(**/*.pem)",
      "Write(.env*)",
      "Write(**/secrets/**)",
      "Bash(git push:*)",
      "Bash(git commit:*)",
      "Bash(git reset:*)",
      "Bash(git rebase:*)",
      "Bash(npm uninstall:*)",
      "Bash(npm remove:*)",
      "Bash(psql:*)",
      "Bash(mysql:*)",
      "Bash(mongod:*)",
      "SQL(DROP TABLE *)",
      "SQL(TRUNCATE TABLE *)",
      "SQL(DELETE FROM *)",
      "mcp__supabase__execute_sql"
    ]
  },
  "enforcePermissions": true,
  "defaultCommandConfirmation": true,
  "displayWarnings": true,
  "safeMode": true
}
---

## ✅ 次のステップ（今後）

1. PCでClaude Codeを使うときにこの内容を `.claude/settings.json` として保存
2. Claudeに「この設定を使って動いて」と指示
3. 必要に応じて内容をアップデート（Obsidianで編集）

---

これで準備万端です。  
このあと「README.md 作りたい」「GitHubにアップしたい」「Claudeに渡してテストしたい」など、次に進む準備も整いました！

どうしますか？次の一歩を一緒に進めましょうか？