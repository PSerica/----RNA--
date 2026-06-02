山雀储食行为相关基因表达调控研究
本项目基于转录组测序数据，系统分析三种山雀（沼泽山雀/储食、黄腹山雀/特殊储食、大山雀/不储食）五个不同部位脑组织的基因表达差异，旨在揭示储食行为进化的分子调控机制。

一、项目概览
研究对象：3种山雀，每种多个生物学重复

分析目标：识别与储食行为强度相关的差异表达基因、共表达网络模块及关键通路

分析方法：DESeq2差异表达 + 有序趋势分析 + WGCNA共表达网络 + GO/KEGG富集分析

技术栈：R (DESeq2, WGCNA, clusterProfiler, ggplot2 等)

├── analysis_config.R                    # 统一分析配置（颜色、阈值、参数）
├── 1.DESeq2_(1).R                       # DESeq2差异表达分析
├── 2.趋势分析(3).R                      # 储食行为有序趋势分析（完整版）
├── 2.趋势分析（改）.R                   # 储食行为有序趋势分析（精简版）
├── 3.WGCNA1-0.R                         # WGCNA共表达网络构建与分析
├── 4.GO_1.R                             # GO富集分析数据准备
├── 5.GO_2.R                             # GO富集分析执行
├── 6.GO_3.R                             # 方法学比较分析
├── 7.KEGG_1.R                           # KEGG通路分析
├── 8.物种特异性基因_3.R                 # 物种特异性基因识别
├── 9.共同差异基因2.R                    # 跨方法保守差异基因分析
│
├── DESeq2_Results/                      # DESeq2分析输出
├── Trend_Analysis_Results/              # 趋势分析结果
├── WGCNA_Results/                       # WGCNA模块、枢纽基因
├── GO_Analysis/                         # GO富集结果
├── Network_Analysis/                    # 网络分析数据
├── Trend_Visualizations/                # 趋势分析可视化
└── WGCNA_Visualizations/                # WGCNA可视化
