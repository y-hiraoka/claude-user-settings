# Claude User Settings

Claude Code のユーザーレベル設定を共有するリポジトリ。

## 含まれるファイル

- `settings.json` - ユーザー設定
- `keybindings.json` - キーバインド設定
- `skills/` - カスタムスキル

## セットアップ

リポジトリをクローンし、各ファイル・ディレクトリを `~/.claude` にシンボリックリンクで配置する。

```bash
git clone https://github.com/y-hiraoka/claude-user-settings.git
cd claude-user-settings

ln -sf "$(pwd)/settings.json" ~/.claude/settings.json
ln -sf "$(pwd)/keybindings.json" ~/.claude/keybindings.json
ln -sf "$(pwd)/skills" ~/.claude/skills
```

既存のファイルがある場合は、必要に応じてバックアップを取ってからリンクを作成すること。

```bash
# バックアップ例
cp ~/.claude/settings.json ~/.claude/settings.json.bak
cp ~/.claude/keybindings.json ~/.claude/keybindings.json.bak
cp -r ~/.claude/skills ~/.claude/skills.bak
```
