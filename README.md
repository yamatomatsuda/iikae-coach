# iikae-skills

職場のメール・チャット・発言を「感じの良い言い方」に直すための、日本語の Claude スキル集です。

| スキル | 使いどころ |
|---|---|
| **iikae-coach** | 文章全体を、相手を見て状況に焦点を当てる言い方に言い換える。場面（依頼・指摘・断り・報告など）と相手との関係を読み取って直す。 |
| **kotoba-check** | 「否定形・相手を下げる前置き・曖昧語・謝罪・催促」の5観点と要チェック語で文章を点検し、引っかかった箇所だけ直す。 |

## 使い方の例

```
この返信、iikae-coachで直して：
「なんで昨日までに出してないんですか？早めにお願いします」
```

```
kotoba-checkして：
「とりあえず送っておきます。一応確認しておいてください」
```

## インストール

### Claude Code（プラグインとして）
```
/plugin marketplace add yamatomatsuda/iikae-coach
/plugin install iikae-skills@iikae-skills
```

### Claude Code（個人スキルとして）
`skills/` 配下のフォルダを `~/.claude/skills/` にコピーしてください。

### Claude.ai / Claude アプリ
`skills/iikae-coach` または `skills/kotoba-check` フォルダを ZIP にして、設定のスキル画面からアップロードしてください。

## 構成

```
skills/
├── iikae-coach/SKILL.md
└── kotoba-check/SKILL.md
.claude-plugin/
├── marketplace.json
└── plugin.json
```

## 方針

- 伝えたい中身や約束の内容は変えず、伝わり方だけを整えます。
- 問題のない文は無理に直しません。
- 言い換え例はすべてオリジナルです。特定の書籍や発信者の文例は転載していません。

## ライセンス

MIT
