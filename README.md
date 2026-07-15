# AI Job Hunting Mail Agent

就活メールをAIで解析し、GoogleカレンダーとNotionを自動更新するMake.comベースのエージェントです。

## Features

- Gmailの新着メールを自動取得
- Gemini APIで企業名・日時・イベント情報を抽出
- 面接・説明会はGoogleカレンダーへ自動登録
- 選考結果やタスクはNotionへ自動登録
- Routerで内容に応じて処理を自動分岐

## Workflow

```text
Gmail
  ↓
Gemini API
  ↓
JSON Parser
  ↓
Router
├─ Google Calendar
└─ Notion
```

## Tech Stack

- Make.com
- Gemini API
- Gmail API
- Google Calendar API
- Notion API

## Import

1. `blueprints/` 内のBlueprint（`.json`）をダウンロード
2. Make.comで **Import Blueprint** を選択
3. `.json` をアップロード
4. 各API（Gmail・Gemini・Google Calendar・Notion）を接続
