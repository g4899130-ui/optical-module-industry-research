# AI 算力驱动下的光模块行业研究

个人独立研究作品，聚焦高速光模块产业链、需求情景、竞争格局和三家上市公司的财务表现。

> 本项目仅用于研究和求职作品展示，不代表任何机构观点，也不构成投资建议。需求测算为情景指数模型，不是市场规模或公司业绩预测。

## 项目概览

- **研究范围：** AI 数据中心 scale-out 网络中的 400G、800G、1.6T 可插拔光模块；排除电信、DCI、铜缆、AOC 整缆、CPO 与 scale-up。
- **研究期间：** 财务数据覆盖 2023—2025 年；资料核查截至 2026-10-08。
- **需求模型：** 以 2025 年为 100 的指数化情景模型；中性情景下 2027 年相对金额指数为 144.7。参数为研究假设，不代表市场事实。
- **公司分析：** 中际旭创、新易盛、光迅科技；包含财务指标、趋势图、风险筛查和权重敏感性分析。

## 文件导航

- [行业研究报告 PDF](report/AI光模块行业研究.pdf)
- [需求测算模型](research/光模块需求测算模型.xlsx)
- [产业链与竞争格局底稿](research/光模块产业链与竞争格局.xlsx)
- [财务口径核查表](research/财务口径核查表.xlsx)
- [研究方法与模型边界](research/METHODOLOGY.md)
- [来源核查清单](research/SOURCE_CHECKLIST.md)
- [Python 财务分析 Notebook](analysis/notebooks/光模块行业财务分析.ipynb)
- [Python 财务分析结果](analysis/outputs/光模块_Python分析结果.xlsx)
- [收入趋势图](analysis/outputs/营业收入趋势.png) · [净利润趋势图](analysis/outputs/归母净利润趋势.png) · [ROE 趋势图](analysis/outputs/ROE趋势.png)

## 复现 Python 分析

需要 Python 3.10 或以上版本。进入 `analysis` 目录，安装依赖并启动 Jupyter：

```bash
python -m pip install -r requirements.txt
jupyter notebook notebooks/光模块行业财务分析.ipynb
```

Notebook 从 `analysis/data/光模块财务数据.xlsx` 读取整理后的财务数据，并在 `analysis/outputs/` 中生成结果表和三张图。运行前请确认已安装 Excel 读写与绘图依赖。

## 口径与限制

财务指标基于公开年报整理；合并毛利率按营业收入和营业成本复算。新易盛 2023—2024 年 ROE 使用 2025 年年报调整后的比较数，具体可比性限制见核查表与方法说明。需求增速、速率份额、相对价值和降价均为情景假设。三家公司、三年数据和有限权重方案不足以支持概率结论或投资决策。

## 公开材料范围

仓库仅保留作品报告、研究底稿、整理后的财务数据、Notebook 和分析结果；未包含原始备份、旧版本 ZIP、内部审计日志或个人简历材料。

