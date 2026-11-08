---
license: cc-by-4.0
language:
- en
- tr
pretty_name: Bulut Doctrine Wikibase Export
tags:
- knowledge-graph
- wikibase
- narratology
- objective-projection
size_categories:
- n<1K
---

# Bulut Doctrine Wikibase Export

This dataset is a JSON export of **leventbulut.wikibase.cloud**, the personal Wikibase instance of Levent Bulut, a former journalist, author and the founder of the Objective Projection method. The instance is not reachable by search-engine crawlers because of the hosting provider's bot protection, so its contents are mirrored here.

The `url` field and the ID links below point to the original records on the Wikibase. They are kept as the source of each record, even though the Wikibase itself is not crawlable; the full content of every record is in the files here.

**This is not Wikidata.** Item numbers (Q1, Q5, …) belong to the leventbulut.wikibase.cloud instance and do not refer to Wikidata items.

## Contents

| File | Description |
|---|---|
| `entities.json` | All 49 items and 25 properties as one JSON array |
| `entities.jsonl` | The same records, one entity per line |

Each record has: `id`, `type` (item or property), `url` (page on the Wikibase), `labels`, `descriptions`, `aliases` (by language code), and `claims`. Each claim lists the `property`, its label, the `values` (an item reference with its label, or a literal value), `qualifiers` and `references`.

## How this export was made

The data was exported on 7 November 2026 with the SPARQL query `SELECT * WHERE { ?s ?p ?o }` on the instance's query service and converted with a short Python script. On the same day, a list of corrections was made on the Wikibase itself (updated descriptions, corrected DOIs and DOI links, `author` instead of `creator of` on two items, removal of one unused property and of DOIs that pointed to unrelated records). A fresh export after those edits failed for technical reasons, so the documented corrections were applied to the earlier export. A new export will replace these files once the query service works again; any difference between the files and the live Wikibase should be read in favour of the live Wikibase.

## Items

| ID | Label (EN) | Label (TR) | Description |
|---|---|---|---|
| [Q1](https://leventbulut.wikibase.cloud/wiki/Item:Q1) | Levent Bulut | Levent Bulut | Former journalist, author and founder of the Objective Projection method; independent researcher working on narrative theory and AI-assisted writing. |
| [Q2](https://leventbulut.wikibase.cloud/wiki/Item:Q2) | human |  | individual member of the species Homo sapiens |
| [Q3](https://leventbulut.wikibase.cloud/wiki/Item:Q3) | researcher |  | person who conducts research or systematic investigation |
| [Q4](https://leventbulut.wikibase.cloud/wiki/Item:Q4) | author |  | person who creates or writes books, articles, or other works |
| [Q5](https://leventbulut.wikibase.cloud/wiki/Item:Q5) | Bulut Doctrine | Bulut Doktrini | A doctrine developed by Levent Bulut that models narrative construction through physical variables and objective projection. |
| [Q6](https://leventbulut.wikibase.cloud/wiki/Item:Q6) | Physics of Literature | Edebiyatın Fiziği | A philosophy developed by Levent Bulut for understanding literature through physical variables and their structural effects on narrative. |
| [Q7](https://leventbulut.wikibase.cloud/wiki/Item:Q7) | Objective Projection | Nesnel İzdüşüm | A narrative method developed by Levent Bulut for representing emotion, meaning, and internal states through observable physical evidence. |
| [Q8](https://leventbulut.wikibase.cloud/wiki/Item:Q8) | Narrative Engineering | Anlatı Mühendisliği | A methodology developed by Levent Bulut for the systematic analysis and construction of narrative structures. |
| [Q9](https://leventbulut.wikibase.cloud/wiki/Item:Q9) | Narrative Entropy | Anlatı Entropisi | A proposed metric by Levent Bulut for information flow and structural complexity in narrative (Sₙ = ∫(If×Cb)dt); no canonical scale has been fixed. |
| [Q10](https://leventbulut.wikibase.cloud/wiki/Item:Q10) | Information Friction | Bilgi Sürtünmesi | A concept developed by Levent Bulut describing the resistance or obstruction affecting the flow of information within a narrative. |
| [Q11](https://leventbulut.wikibase.cloud/wiki/Item:Q11) | Narrative Momentum | Anlatı Momentumu | A concept developed by Levent Bulut describing the temporal dimension of objective projection and the dynamic progression of narrative structure. |
| [Q12](https://leventbulut.wikibase.cloud/wiki/Item:Q12) | Narrative Inertia | Anlatı Eylemsizliği | A concept developed by Levent Bulut describing the persistence of established narrative patterns and information structures over time. |
| [Q13](https://leventbulut.wikibase.cloud/wiki/Item:Q13) | Canonical Narrative Entropy | Kanonik Anlatı Entropisi | A formulation developed by Levent Bulut for modeling entropy within a canonical narrative structure. |
| [Q14](https://leventbulut.wikibase.cloud/wiki/Item:Q14) | THE BULUT DOCTRINE v2026 | Bulut Doktrini v2026 | Extended manifesto by Levent Bulut on narrative construction (2026). |
| [Q15](https://leventbulut.wikibase.cloud/wiki/Item:Q15) | Turkish | Türkçe | natural language spoken in Turkey |
| [Q16](https://leventbulut.wikibase.cloud/wiki/Item:Q16) | English |  | language |
| [Q17](https://leventbulut.wikibase.cloud/wiki/Item:Q17) | Bilim Gönül Yayınları |  | publishing house |
| [Q18](https://leventbulut.wikibase.cloud/wiki/Item:Q18) | İştirak Yayınları |  | publishing house |
| [Q19](https://leventbulut.wikibase.cloud/wiki/Item:Q19) | KDY |  | Kitapyurdu Doğrudan Yayıncılık |
| [Q20](https://leventbulut.wikibase.cloud/wiki/Item:Q20) | Levent Bulut |  | independent publisher |
| [Q21](https://leventbulut.wikibase.cloud/wiki/Item:Q21) | Darağacı: Türkiye-İran Suriye | Darağacı: Türkiye-İran Suriye | book by Levent Bulut |
| [Q22](https://leventbulut.wikibase.cloud/wiki/Item:Q22) | book | kitap | written publication |
| [Q23](https://leventbulut.wikibase.cloud/wiki/Item:Q23) | Utanın | Utanın | book by Levent Bulut |
| [Q24](https://leventbulut.wikibase.cloud/wiki/Item:Q24) | Haberin Peşinde: Gazetecinin El Kitabı | Haberin Peşinde: Gazetecinin El Kitabı | book by Levent Bulut |
| [Q25](https://leventbulut.wikibase.cloud/wiki/Item:Q25) | Veri ve Hayalet | Veri ve Hayalet | book by Levent Bulut |
| [Q26](https://leventbulut.wikibase.cloud/wiki/Item:Q26) | Doğruya Doğru: Bir Gazetecinin Seyir Defteri | Doğruya Doğru: Bir Gazetecinin Seyir Defteri | book by Levent Bulut |
| [Q27](https://leventbulut.wikibase.cloud/wiki/Item:Q27) | Ayça'nın Kelimesiz Dünyası | Ayça'nın Kelimesiz Dünyası | book by Levent Bulut |
| [Q28](https://leventbulut.wikibase.cloud/wiki/Item:Q28) | Nesnel İzdüşüm: Beş Sahne ve Bir Teknik | Nesnel İzdüşüm: Beş Sahne ve Bir Teknik | e-book by Levent Bulut |
| [Q29](https://leventbulut.wikibase.cloud/wiki/Item:Q29) | ANLATININ FİZİĞİ: Beyin, Duygu ve Kelimeler | ANLATININ FİZİĞİ: Beyin, Duygu ve Kelimeler | book by Levent Bulut |
| [Q30](https://leventbulut.wikibase.cloud/wiki/Item:Q30) | Objective Projection: Five Scenes and a Technique | Objective Projection: Five Scenes and a Technique | e-book by Levent Bulut |
| [Q31](https://leventbulut.wikibase.cloud/wiki/Item:Q31) | THE PHYSICS OF NARRATIVE |  | e-book by Levent Bulut |
| [Q32](https://leventbulut.wikibase.cloud/wiki/Item:Q32) | investigative journalist | araştırmacı gazeteci | profession |
| [Q33](https://leventbulut.wikibase.cloud/wiki/Item:Q33) | concept | kavram | abstract unit of knowledge or theoretical construct |
| [Q34](https://leventbulut.wikibase.cloud/wiki/Item:Q34) | Narrative Gravity | Anlatı Kütleçekimi | Qualitative concept by Levent Bulut (Ng) for the structural pull of a narrative element; the earlier formula Ng = Ma/Sₙ² has been withdrawn. |
| [Q35](https://leventbulut.wikibase.cloud/wiki/Item:Q35) | Universal Biological Interface | Evrensel Biyolojik Arayüz | Untested hypothesis by Levent Bulut about how readers process physical sensory detail in narrative. |
| [Q36](https://leventbulut.wikibase.cloud/wiki/Item:Q36) | Summarization Bias | Özetleme Yanlılığı | Untested hypothesis by Levent Bulut that language models summarizing physically written scenes replace physical detail with named emotions (registered protocol). |
| [Q37](https://leventbulut.wikibase.cloud/wiki/Item:Q37) | Biophysical Output | Biyofiziksel Çıktı | Concept by Levent Bulut: observable physical detail written in place of an explicit emotion label. |
| [Q38](https://leventbulut.wikibase.cloud/wiki/Item:Q38) | Causal Branching | Nedensel Dallanma | construct modeling narrative probability pathways and structural divergence |
| [Q39](https://leventbulut.wikibase.cloud/wiki/Item:Q39) | Vacuum Variable | Vakum Değişkeni | Concept by Levent Bulut for gaps in physical detail that leave the reader to infer what is not stated. |
| [Q40](https://leventbulut.wikibase.cloud/wiki/Item:Q40) | Emotion Embargo | Duygu Ambargosu | One of the two constitutional rules of Objective Projection: the narrator does not name emotions and conveys them through physical detail; its documented limits include irony, unreliable narrators and dialogue. |
| [Q41](https://leventbulut.wikibase.cloud/wiki/Item:Q41) | Dokuzsutun | Dokuzsütun Gazetesi | daily newspaper in Turkey |
| [Q42](https://leventbulut.wikibase.cloud/wiki/Item:Q42) | newspaper | gazete | periodical publication containing news |
| [Q43](https://leventbulut.wikibase.cloud/wiki/Item:Q43) | gunboyu | günboyu | daily newspaper in Turkey |
| [Q44](https://leventbulut.wikibase.cloud/wiki/Item:Q44) | Yenicag | Yeniçağ Gazetesi | daily newspaper in Turkey |
| [Q45](https://leventbulut.wikibase.cloud/wiki/Item:Q45) | Istanbul University | İstanbul Üniversitesi | public university in Istanbul, Turkey |
| [Q46](https://leventbulut.wikibase.cloud/wiki/Item:Q46) | Anadolu University | Anadolu Üniversitesi | public university in Eskisehir, Turkey |
| [Q47](https://leventbulut.wikibase.cloud/wiki/Item:Q47) | scholarly article | bilimsel makale | article in an academic publication |
| [Q48](https://leventbulut.wikibase.cloud/wiki/Item:Q48) | OPCT (Objective Projection Calibration Test) | OPCT | Pre-registered calibration test protocol for Objective Projection (OSF us8bw); it has not been run. |
| [Q49](https://leventbulut.wikibase.cloud/wiki/Item:Q49) | Objective Projection Dataset | Nesnel İzdüşüm Veri Seti | Bilingual Turkish–English corpus of 500 scene pairs annotated for Objective Projection craft features; published on Hugging Face. |

## Scope and status

- The Wikibase records what Levent Bulut has published and named. A statement here is a record of that claim, not an independent assessment of it.
- Concepts such as the Universal Biological Interface and Summarization Bias are hypotheses that have not been tested by independent researchers.
- For the current definitions, see https://leventbulut.com/ and the DOIs listed in each record.

## Links

- Website: https://leventbulut.com/
- Knowledge graph page on the website: https://leventbulut.com/graph/
- Corpus of registered works: https://leventbulut.com/corpus/
- ORCID: https://orcid.org/0009-0007-7500-2261
- Main dataset: https://huggingface.co/datasets/leventbulut/objective-projection (DOI 10.57967/hf/8960)
- GitHub mirror of this dataset: https://github.com/levent-bulut/bulut-doctrine-wikibase

## Citation

```bibtex
@misc{bulut_wikibase_export_2026,
  author = {Bulut, Levent},
  title  = {Bulut Doctrine Wikibase Export},
  year   = {2026},
  publisher = {Hugging Face},
  howpublished = {\url{https://huggingface.co/datasets/leventbulut/bulut-doctrine-wikibase}}
}
```
