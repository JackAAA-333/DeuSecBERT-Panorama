# DeuSecBERT-Panorama

面向德语安全与防务话语的领域自适应预训练模型（**DeuSecBERT**），以及"时代转折"（Zeitenwende）背景下德国发展动向的**全景图谱（Panorama Atlas）**解析与预测系列研究。

本仓库是研究计划《德国安全话语计算建模与全景图谱研究计划》（v1.0，2026-10）的配套开源工程，承接已录用论文《德国安全话语体系中军事词汇的隐喻再构研究——基于GBERT语境词向量的源域-目标域语义空间分析（2022-2026）》（德语期刊，稿号 2026-0866）。

## 研究目标

1. **DeuSecBERT**：对 GBERT 进行安全防务领域化改进（DAPT 继续预训练 + 领域词汇扩充 + 时间感知对比学习），并构建隐喻识别、源域-目标域映射、立场/框架检测、语义变化预警、安全事件抽取五类任务的统一基准。
2. **全景图谱系列**：以"全景图谱型"范式穷尽式覆盖国防、外交、经济、能源、科技、对华政策六大专题的多源语料，构建话语图谱、事件图谱、主体网络图谱与指标预测图谱，实现德国政策动向的量化解析与前瞻预测。

## 仓库结构

```
├── README.md
├── LICENSE                      # MIT
├── CITATION.cff
├── requirements.txt
├── docs/
│   ├── RESEARCH_PLAN.md         # 研究计划全文（与PDF版同步）
│   └── CORPORA.md               # 语料库资源清单与申请指南
├── data/                        # 语料与标注数据（遵循各数据源许可）
│   ├── raw/                     # 原始语料获取脚本与清单
│   ├── deseccorpus/             # DeuSecCorpus 领域预训练语料
│   └── annotations/             # DeuSecMeta 等标注集
├── src/
│   ├── corpora/                 # 语料采集、清洗、去重、时间切分
│   ├── pretraining/             # DAPT / 词汇扩充 / 时间感知对比学习
│   ├── tasks/                   # T1-T5 任务实现与评测
│   ├── atlas/                   # 全景图谱：话语/事件/网络/预测四层
│   └── utils/
├── scripts/                     # 可复现实验入口
└── results/                     # 实验结果与图表
```

## 里程碑

| 里程碑 | 时间 | 交付物 |
|---|---|---|
| M0 语料底座 | 2026 Q4 – 2027 Q1 | DeuSecCorpus v1、语料申请完成、基线复现 |
| M1 DeuSecBERT v1 | 2027 Q2 – Q3 | DAPT 模型 + 内在评测报告 |
| M2 任务基准 | 2027 Q3 – 2028 Q1 | DeuSecMeta 标注集 + T1–T3 基准与论文 |
| M3 语义变化预警 | 2028 Q1 – Q2 | T4 语义漂移指数 + ACL/EMNLP 投稿 |
| M4 国防专题图谱 | 2028 Q2 – Q4 | 国防全景图谱 + Dashboard |
| M5 六专题扩展 | 2029 | 外交/经济/能源/科技/对华图谱 + 年度报告 |
| M6 预测模型 | 2029 | 话语先行指标→政策结果预测模型与回测 |

## 主要语料与资源

详见 [docs/CORPORA.md](docs/CORPORA.md)。核心包括：OpenDiscourse（Bundestag 全会语料）、GermaParl、Bundesregierung 演讲档案、BMVg 防务文件（Weißbuch 2016 / Militärische Grundstrategie 2026）、DWDS、DeReKo/COSMAS II、Leipzig Corpora Collection、OSCAR、GDELT 2.0、Manifesto Corpus、German Political Speeches Corpus、SIPRI 军费数据库等。

## 合规说明

- 各语料遵循其原始许可协议（CC-BY / CC0 / 学术注册协议 / Nutzungsbedingungen des Deutschen Bundestages 等），`data/` 目录不直接再分发受限语料，仅提供获取脚本与清单。
- 研究输出仅用于学术研究，不构成任何政策或投资建议。

## 引用

```bibtex
@misc{desecbert_panorama_2026,
  title  = {DeuSecBERT-Panorama: 德国安全话语计算建模与全景图谱研究},
  author = {Shanshan, Liang and Zefang, Li},
  year   = {2026},
  url    = {https://github.com/JackAAA-333/DeuSecBERT-Panorama}
}
```

## 联系方式

梁珊珊（imkeliang@126.com）、李泽芳（lizefang2957@126.com）｜北京理工大学
