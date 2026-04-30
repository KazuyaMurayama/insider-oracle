# FILE_INDEX.md — insider-oracle

> **新セッション開始時に必ずこのファイルを読む。**
> ファイル追加・削除・移動時は必ずこのファイルを更新すること。
> 最終更新: 2026-04-30

## 概要
葛西ワンルーム不動産の確定申告・節税・青色申告対応マルチエージェントシステム。税務調査官・税理士・銀行員・大家の4エージェント構成。

**スタック:** Markdown, JSON, PDF, CSV

---

## 📋 最初に読むべきファイル

| 優先度 | ファイル | 内容 |
|---|---|---|
| ★★★ | `CLAUDE.md` | 運用ルール・エージェント指針 |
| ★★★ | `README.md` | システム概要・使い方 |
| ★★★ | `agents/` | 4エージェント定義（必読） |
| ★★ | `properties/kasai_rc_603.json` | 葛西物件マスターデータ |
| ★★ | `outputs/` | 申告ガイド・節税戦略レポート |

---

## 🗂️ ディレクトリ構造

```
insider-oracle/
├── CLAUDE.md                    ← 最重要ルール
├── README.md
├── agents/
│   ├── agent_a_tax_inspector.md ← 税務調査官エージェント
│   ├── agent_b_tax_accountant.md← 税理士エージェント
│   ├── agent_c_bank_officer.md  ← 銀行員エージェント
│   └── agent_d_landlord.md      ← 大家エージェント
├── knowledge/
│   ├── tax/
│   │   ├── expense_catalog.md
│   │   ├── investigation_cases.md
│   │   ├── tax_rate_table.md
│   │   └── tax_updates.md
│   └── realestate/
│       ├── dead_cross_model.md
│       └── depreciation_guide.md
├── properties/
│   ├── index.json
│   └── kasai_rc_603.json        ← 葛西物件マスター
├── records/2026/                ← 2026年度経費記録
│   ├── transport_log.csv
│   ├── bank_fees_log.csv
│   ├── supplies_log.csv
│   ├── entertainment_log.csv
│   ├── books_seminars_log.csv
│   ├── depreciation_calculation_basis.md
│   ├── home_office_basis.md
│   └── property_visit_notes.md
├── outputs/
│   ├── 20260310_kasai_2026_tax_filing_guide.md
│   ├── 20260310_kasai_tax_saving_strategies.md
│   ├── 20260311_blue_return_application_guide.md
│   ├── 所得税の青色申告承認申請書.pdf
│   └── 青色申告承認申請書_記入済み.pdf
└── state/session.json
```

---

## 📑 全ファイル一覧

| パス | 種別 | 説明 |
|---|---|---|
| `CLAUDE.md` | ドキュメント | 運用ルール・エージェント指針 |
| `README.md` | ドキュメント | システム概要・使い方 |
| `agents/agent_a_tax_inspector.md` | エージェント | 税務調査官エージェント定義 |
| `agents/agent_b_tax_accountant.md` | エージェント | 税理士エージェント定義 |
| `agents/agent_c_bank_officer.md` | エージェント | 銀行員エージェント定義 |
| `agents/agent_d_landlord.md` | エージェント | 大家エージェント定義 |
| `knowledge/tax/expense_catalog.md` | 知識 | 経費カタログ |
| `knowledge/tax/tax_rate_table.md` | 知識 | 税率表 |
| `knowledge/realestate/depreciation_guide.md` | 知識 | 減価償却ガイド |
| `properties/kasai_rc_603.json` | データ | 葛西物件マスターデータ |
| `records/2026/transport_log.csv` | データ | 2026年交通費ログ |
| `records/2026/depreciation_calculation_basis.md` | ドキュメント | 減価償却計算根拠 |
| `outputs/20260310_kasai_2026_tax_filing_guide.md` | レポート | 2026年確定申告ガイド |
| `outputs/20260310_kasai_tax_saving_strategies.md` | レポート | 節税戦略レポート |
| `outputs/20260311_blue_return_application_guide.md` | レポート | 青色申告承認申請ガイド |
| `state/session.json` | データ | セッション状態 |

---

## 🔖 ファイル更新ルール

1. 新ファイル追加時: 該当セクションに1行追加
2. ファイル削除・移動時: 該当行を削除または更新
3. 更新後: `git add FILE_INDEX.md && git commit -m "docs: FILE_INDEX.md更新"`
