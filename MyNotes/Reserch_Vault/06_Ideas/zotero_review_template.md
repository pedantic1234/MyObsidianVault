---
title: "{{title}}"
authors: "{{authors}}"
year: {{date | format("YYYY")}}
citekey: "{{citekey}}"
tags:
  - literature
  - review
  - review-paper
---

# {{title}}

## 📚 論文情報
- **著者**: {{authors}}
- **発表年**: {{date | format("YYYY")}}
- **雑誌**: {{publicationTitle}}
- **DOI**: {{DOI}}
- **Zotero**: [Open in Zotero]({{zoteroSelectURI}})
- **PDF**: {% if attachments %}[📄 PDF]({{attachments[0].path}}){% endif %}

## 🔖 Citation Key
`{{citekey}}`

## 🏷️ Zoteroタグ
{% for tag in tags -%}
#{{tag.tag | replace(" ", "_")}}{% if not loop.last %}, {% endif %}
{% endfor -%}

## 🔬 アブストラクト
{{abstractNote}}

## 📝 3行要約
- **対象領域**: 
- **主要論点**: 
- **結論**: 

## 📖 レビュー構造の整理

### カバーしている主要トピック
1. 
2. 
3. 

### 各トピックの概要

#### トピック1: 
- **主要知見**: 
- **エビデンスレベル**: 
- **議論の余地**: 

#### トピック2: 
- **主要知見**: 
- **エビデンスレベル**: 
- **議論の余地**: 

## 🔍 重要な知見まとめ

### 確立された知見（コンセンサス）
- 

### 論争のある領域
- 

### 未解明の課題
- 

## 🌐 分野全体における位置づけ
- 

## 📊 引用されている重要研究

### 必読論文リスト
1. [[]] - 
2. [[]] - 
3. [[]] - 

### 重要な実験的証拠
- 

## 💭 批判的評価

### レビューの強み
- 

### レビューの限界
- 

### 偏りや不足している視点
- 

## 🎯 自分の研究への示唆
- 

## 💡 今後の研究方向性
### このレビューが示唆する研究機会
- 

### 自分のアイデア
- 

---
**作成日**: {{date | format("YYYY-MM-DD")}}
**再レビュー予定**: {{date+30d | format("YYYY-MM-DD")}}
