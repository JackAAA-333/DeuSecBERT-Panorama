# data/

本目录用于存放语料与标注数据。**注意**：受限语料（DWDS、DeReKo、GermaNet、GermEval 等）不在仓库中再分发，
仅保存获取脚本（`raw/`）、清单（manifest）与派生统计结果；各文件遵循原始许可协议。

- `raw/`：各数据源下载与预处理脚本 + manifest.yaml（来源、许可、版本、获取日期）
- `deseccorpus/`：DeuSecCorpus 领域预训练语料的构建流水线输出（去重、时间切分后）
- `annotations/`：DeuSecMeta 隐喻标注、框架标注等（拟以 CC-BY 4.0 发布）
