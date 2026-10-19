# visor-catalog

[visor](https://github.com/MoomA-0750/visor) の公式のアプリのカタログ。visor は `catalog.json` を読み、ホームの「アプリを探す」に並べる。`preinstall` の付いたアプリは、visor を初めて起こしたときに入れる。

## catalog.json

```json
{
  "name": "カタログの名前",
  "apps": [
    { "id": "calendar", "name": "カレンダー", "icon": "calendar_month", "description": "…", "source": "github:owner/repo", "preinstall": true }
  ]
}
```

- `source`: アプリのリポジトリ（`github:owner/repo`、`@ref` でブランチやタグを決められる）。根元に `app.json` がある
- `icon`: Material Symbols のアイコンの名前

アプリの作り方は visor の `docs/extensions.md`。
