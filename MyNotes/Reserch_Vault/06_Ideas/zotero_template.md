---
title: "{{title}}"
authors: "{{authors}}"
year: {{date | format("YYYY")}}
citekey: "{{citekey}}"
tags:
  - literature
  - original-paper
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

## 📝 3行要約
1. **目的**: 
2. **方法**: 
3. **結果**: 

## 🔬 詳細メモ

### 背景・目的
{{abstractNote}}

### 方法論
- **実験対象**: 
- **実験手法**: 
- **解析方法**: 

### 主要結果
- 

### 考察のポイント
- 

## 🎯 研究の意義・応用
- 

## ❓ 批判的検討

### 新規性
- 

### 限界点
- 

### 疑問点
- 

## 🔗 関連研究ネットワーク

### 重要な引用文献
- 

### この論文を引用している研究
- 

### 同分野の比較研究
- 

## 💡 今後の研究アイデア
- 

---
**作成日**: {{date | format("YYYY-MM-DD")}}
**レビュー予定**: {{date+7d | format("YYYY-MM-DD")}}
