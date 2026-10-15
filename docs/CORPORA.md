# 语料库资源清单与申请指南

> 版本 v1.0（2026-10-15）。申请时请以各官网最新条款为准。

## A. 议会与政府语料（核心）

| 资源 | 内容 | 许可/获取 | 申请所需材料 |
|---|---|---|---|
| OpenDiscourse | 1949–2021 联邦议院全会演讲结构化语料 | 开放（GitHub/Zenodo, opendiscourse.de） | 无需申请 |
| Bundestag Open Data / DIP | 全会速记记录、立法草案、表决 | 开放（bundestag.de/services/opendata；dip.bundestag.de） | 无需申请 |
| GermaParl (PolMine) | 联邦议院全会语料（R 生态） | 开放（github.com/PolMine） | 无需申请 |
| Bundesregierung 演讲档案 | 总理/部长演讲、政策声明 | 开放（bundesregierung.de，遵守 Nutzungsbedingungen） | 无需申请 |
| BMVg 防务文件 | Weißbuch 2016、Verteidigungspolitische Richtlinien 2023、Militärische Grundstrategie 2026 | 开放（bmvg.de） | 无需申请 |
| Corpus der Drucksachen (CDRS-BT) | 联邦议院印刷文件 2.9 亿词 | CC0（Zenodo 4643066） | 无需申请 |

## B. 通用与新闻语料

| 资源 | 内容 | 许可/获取 | 申请所需材料 |
|---|---|---|---|
| DWDS | 核心语料+新闻/博客子语料、历时检索 | dwds.de 免费注册；部分子语料需签署学术使用许可 | 注册账号；部分语料需提交机构、研究用途说明并签署许可协议 |
| DeReKo / COSMAS II | IDS 现代德语参考语料库（百亿词级） | cosmas2.ids-mannheim.de 免费注册，学术用途 | 注册账号，说明研究项目；批量下载需向 IDS 申请 |
| Leipzig Corpora Collection | 标准规模新闻/网页语料（1万–100万句） | CC-BY 4.0（wortschatz.uni-leipzig.de） | 无需申请 |
| OSCAR / German Commons | Common Crawl 德语语料（145GB+ / 154B tokens） | HF/官网公开下载 | 无需申请 |
| GDELT 2.0（GKG/Events） | 全球新闻事件与知识图谱（含德语流） | 开放（gdeltproject.org；BigQuery） | 无需申请（BigQuery 需 Google 账号） |
| German Political Speeches Corpus | 2019 整理的德语政治演讲集 | CC-BY 4.0（Zenodo 3611246） | 无需申请 |
| Manifesto Corpus | 67 国政党竞选纲领准句级人工编码 | 注册 API key（manifesto-project.wzb.eu，学术邮箱） | 注册账号+学术邮箱验证 |
| SIPRI Military Expenditure | 全球军费数据库 | 开放（sipri.org） | 无需申请 |

## C. 评测与标注资源

| 资源 | 内容 | 获取 |
|---|---|---|
| SemEval-2020 Task 1 | 词汇语义变化检测（含德语子任务） | github.com/CHANGE-2020 公开 |
| GermEval 系列 | NER 2014、情绪 2017/2018/2019、仇恨言论 2021 等 | 各年官网注册 |
| DWUG（DURel） | 德语语义变化人工标注词表 | github.com/Garrafao 公开 |
| GermaNet | 德语词汇语义网 | uni-tuebingen 学术许可协议（在线签署） |
| DTA | 德语历史文本档案 | 开放（deutschestextarchiv.de） |
| Europarl / OPUS | 欧洲议会平行语料 | 开放（opus.nlpl.eu） |

## D. 自建采集（合规要点）

- GDELT GKG 德语子流：按 `language=German` 过滤，遵守 GDELT 使用条款。
- Bundestag/DIP 官方 API：遵守 §4 Archivordnung 与 robots 条款。
- 自建标注集 DeuSecMeta：按 MIPVU 规范双人标注，报告 Cohen's κ 与 adjudication 流程。
