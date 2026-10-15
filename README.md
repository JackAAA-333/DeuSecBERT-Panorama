# DeuSecBERT-Panorama

面向德语安全与防务话语的领域自适应模型（**DeuSecBERT**）、普惠德语研究工具链，以及完整的**德国跨文化计算研究方法论**。

本仓库是研究计划《面向顶会与普惠工具的德国跨文化计算研究计划》（v2.0，2026-10）的配套开源工程，承接已录用论文《德国安全话语体系中军事词汇的隐喻再构研究——基于GBERT语境词向量的源域-目标域语义空间分析（2022-2026）》（德语期刊，稿号 2026-0866）。

## 三大目标

1. **顶会成果**：在 ACL / EMNLP / NAACL / COLING / LREC（含 Findings、评测与 Demo）形成"模型—数据集—方法—工具"论文序列。
2. **普惠德语研究工具（让每个人都能用）**：DeuSec-Toolkit（pip 包）、Web 在线工具、REST API、中英德三语教程与 Notebook 模板；无需机器学习背景即可分析德语文本的隐喻、框架、立场与语义漂移。
3. **完整的德国跨文化研究方法论**：借鉴"全景图谱型"研究的 AI 方法论内核（穷尽覆盖 × 统一坐标 × 表征学习 × 全量关联扫描 × 纵向预测），构建"全景解析 → 跨文化比较 → 六步方法规程"三层体系（见 [docs/METHODOLOGY.md](docs/METHODOLOGY.md)）。

> AI 的价值主张：让严谨方法难以量化的对象——隐喻、框架、立场、文化认知——可量化、可复现、有迹可循（每个指标可回溯到具体文本证据）。

## 两大方向

- **方向一 DeuSecBERT**：GBERT 领域化改进（DAPT 继续预训练 + 军事术语词汇扩充 + 时间感知对比学习），五任务统一基准 T1–T5（隐喻识别 / 源-目标域映射 / 立场与框架 / 语义变化预警 / 安全事件抽取）。
- **方向二 全景解析与跨文化比较**：国防、外交、经济、能源、科技、对华政策六专题 × 话语/事件/主体网络/指标预测四层图谱；以德语为中心锚定汉语/英语语义空间，开展德中、德美、德法跨文化话语比较。

## 仓库结构

```
├── README.md / LICENSE(MIT) / CITATION.cff / requirements.txt
├── docs/
│   ├── RESEARCH_PLAN.md         # 研究计划（与 PDF 版同步）
│   ├── CORPORA.md               # 语料库资源清单与申请指南
│   └── METHODOLOGY.md           # 德国跨文化计算研究方法论（六步规程）
├── data/                        # 语料与标注（遵循各数据源许可）
│   ├── raw/                     # 获取脚本 + manifest
│   ├── deseccorpus/             # DeuSecCorpus 领域预训练语料
│   └── annotations/             # DeuSecMeta 等标注集
├── src/
│   ├── corpora/                 # 语料采集、清洗、去重、按月切分
│   ├── pretraining/             # DAPT / 词汇扩充 / 时间感知对比学习
│   ├── tasks/                   # T1–T5 任务实现与评测
│   ├── atlas/                   # 全景图谱四层 + 跨语言对齐
│   └── utils/
├── toolkit/                     # DeuSec-Toolkit（pip）· web（Web/API）· tutorials
├── scripts/                     # 可复现实验入口
└── results/                     # 评测报告与图表
```

## 里程碑（2026Q4–2029Q4）

| 里程碑 | 时间 | 交付物 |
|---|---|---|
| M0 语料底座 | 2026 Q4 – 2027 Q1 | DeuSecCorpus v1、语料申请完成、基线复现 |
| M1 DeuSecBERT v1 | 2027 Q2 – Q3 | DAPT 三初始化对比 + 词汇扩充 + 内在评测 |
| M2 任务基准 | 2027 Q3 – 2028 Q1 | DeuSecMeta + T1–T5 基准；模型/数据集论文投稿 |
| M3 跨语言对齐 | 2028 Q1 – Q3 | 德中/德美/德法语义对齐；跨文化比较论文 |
| M4 工具平台 | 2028 Q3 – 2029 Q1 | DeuSec-Toolkit + Web/API + 教程；Demo 论文投稿 |
| M5 全景图谱 | 2028 Q4 – 2029 Q3 | 国防首发 → 六专题图谱；年度报告与看板 |
| M6 方法论与预测 | 2029 | 跨文化方法论手册；先行指标预测模型与回测 |

## 合规说明

- 各语料遵循其原始许可协议（CC-BY / CC0 / 学术注册协议等），`data/` 目录不直接再分发受限语料，仅提供获取脚本与清单。
- 研究输出仅用于学术研究，不构成任何政策或投资建议。

## 引用

```bibtex
@misc{desecbert_panorama_2026,
  title  = {DeuSecBERT-Panorama: 面向顶会与普惠工具的德国跨文化计算研究},
  author = {Shanshan, Liang and Zefang, Li},
  year   = {2026},
  url    = {https://github.com/JackAAA-333/DeuSecBERT-Panorama}
}
```

## 联系方式

梁珊珊（imkeliang@126.com）、李泽芳（lizefang2957@126.com）｜北京理工大学
