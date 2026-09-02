<div align="center">

# 可信无线通信自动研究

### 从宽泛研究方向到有证据支撑的完整论文

[English](README.md) | [中文](README.zh-CN.md)

<p>
  <a href="LICENSE"><img alt="许可证：CC BY 4.0" src="https://img.shields.io/badge/许可证-CC%20BY%204.0-2f6f9f?style=flat-square"></a>
  <img alt="研究流程" src="https://img.shields.io/badge/研究流程-5%20个证据门-0969da?style=flat-square">
  <img alt="候选选题" src="https://img.shields.io/badge/候选选题-70-8250df?style=flat-square">
  <img alt="研究领域" src="https://img.shields.io/badge/案例-UAV--ISAC-1a7f37?style=flat-square">
</p>

本仓库以 **“ISAC for UAVs”** 为起点，呈现一条涵盖文献调研、研究构想、物理建模、优化设计、仿真验证、证据综合与论文级评估的端到端研究证据链。

[总体框架](Trustworthy_Wireless_AutoResearch_Framework.pdf) · [70 个选题](Literature_Review_and_Research_Idea_Generation/00_overall_70_idea_report.pdf) · [选定题目](Selected_Research_Topic.pdf) · [案例论文](Near_Field_ISAC_for_Six_Dimensional_UAV_Pose_Estimation.pdf) · [仿真结果](Simulation_Experimentation_and_Result_Generation/)

<a href="Trustworthy_Wireless_AutoResearch_Framework.pdf">
  <img src="assets/framework_overview.gif" alt="包含 Human Check Gate 通过与返回机制的可信无线通信自动研究五阶段动态流程" width="100%">
</a>

<sub>在每个 Human Check Gate，未通过的研究产物会返回当前阶段修改，通过后再进入下一阶段；点击动画可查看矢量 PDF。</sub>

</div>

## 🧭 项目概览

| 初始方向 | 文献证据 | 候选空间 | 评价方式 | 最终案例 |
|---|---:|---:|---|---|
| ISAC for UAVs | 434 条检索记录 | 70 个研究题目 | 8 个加权维度 | 面向六维无人机位姿估计的近场 ISAC |

这里展示的不是零散的生成文件，而是一条可以检查的**研究证据链**。每一阶段都会产生明确的研究产物，并在可配置的人类监督下通过验证、定向修改，或返回上游阶段。

## 🔬 五阶段研究证据链

| 阶段 | 核心问题 | 仓库中的证据 |
|---|---|---|
| **1. 文献调研与研究构想生成** | 什么问题值得研究，研究缺口是否成立？ | [调研文献库](Surveyed_Literature_Corpus_for_UAV_ISAC.pdf)、[70 个候选题目](Literature_Review_and_Research_Idea_Generation/00_overall_70_idea_report.pdf)、[排名表](UAV_ISAC_Research_Topic_Ranking.pdf)、[分项评分表](UAV_ISAC_Component_Scores.pdf)以及[全部选题简报](Literature_Review_and_Research_Idea_Generation/candidate_research_ideas/) |
| **2. 系统建模与基本极限分析** | 在既定物理假设和干扰参数下，研究命题是否成立？ | [选定研究问题](Selected_Research_Topic.pdf)及[案例论文](Near_Field_ISAC_for_Six_Dimensional_UAV_Pose_Estimation.pdf)中的系统模型与 CRB 分析 |
| **3. 问题构建与系统优化** | 如何配置通信与感知资源？ | [案例论文](Near_Field_ISAC_for_Six_Dimensional_UAV_Pose_Estimation.pdf)中的位姿感知优化、可辨识性分析、SDP 重构与估计算法 |
| **4. 仿真、实验与结果生成** | 理论、算法和公平基线在一致条件下是否相互吻合？ | [通信速率-位姿精度权衡](Simulation_Experimentation_and_Result_Generation/fig_rate_pose_tradeoff.pdf)、[位置 RMSE](Simulation_Experimentation_and_Result_Generation/fig_position_rmse.pdf)、[姿态 RMSE](Simulation_Experimentation_and_Result_Generation/fig_orientation_rmse.pdf)和[降落轨迹](Simulation_Experimentation_and_Result_Generation/fig_landing_trajectory.pdf) |
| **5. 科学洞见综合与论文准备** | 最终结论是否得到证据支持，并与最相关工作正确对比？ | [最终案例论文](Near_Field_ISAC_for_Six_Dimensional_UAV_Pose_Estimation.pdf)及[IEEE conference/letter 对比表](Compared_IEEE_Conference_and_Letter_Papers.pdf) |

## ✈️ 代表性案例

### Near-Field ISAC for Six-Dimensional UAV Pose Estimation During Landing

该研究考虑单基地 XL 阵列基站：在维持通信链路的同时，对降落无人机上的校准编码标志点进行探测。精确球面波响应与刚体几何关系将三维位置和三维姿态统一到同一个位姿估计问题中。

论文形成了以下主要技术产物：

- 消除未知反射系数后的位姿信息分析与 Cramér-Rao bound；
- 六维位姿局部可辨识条件；
- 面向位姿精度的通信-感知功率分配问题；
- 用于绝对无人机位姿恢复的变量投影估计方法。

## 📚 主要材料入口

| 材料 | 内容 |
|---|---|
| [总体框架](Trustworthy_Wireless_AutoResearch_Framework.pdf) | 五阶段研究流程、验证门与人类监督机制 |
| [70 个候选题目报告](Literature_Review_and_Research_Idea_Generation/00_overall_70_idea_report.pdf) | 全部候选 UAV-ISAC 研究题目及排名 |
| [候选题目文件夹](Literature_Review_and_Research_Idea_Generation/candidate_research_ideas/) | Rank 01–70 的独立研究简报 |
| [题目排名表](UAV_ISAC_Research_Topic_Ranking.pdf) | Rank、score 与题目的紧凑表格 |
| [分项评分表](UAV_ISAC_Component_Scores.pdf) | 八个评价维度的分项结果 |
| [调研文献库](Surveyed_Literature_Corpus_for_UAV_ISAC.pdf) | 研究构想生成阶段使用的可检索文献证据 |
| [案例论文](Near_Field_ISAC_for_Six_Dimensional_UAV_Pose_Estimation.pdf) | 从选定题目形成的完整研究成果 |
| [相关论文对比表](Compared_IEEE_Conference_and_Letter_Papers.pdf) | 五篇 IEEE ICC/GLOBECOM 论文和五篇 IEEE letters |
| [仿真结果图](Simulation_Experimentation_and_Result_Generation/) | 四张论文中的数值结果图 |

## 📄 许可证与署名

本仓库汇集了无线通信 AutoResearch 总体框架、调研文献库、70 个候选研究题目及其评价表、选定的近场 UAV-ISAC 案例论文、已发表论文对比表，以及论文中的数值仿真结果图。

除非另有说明，本仓库中由 **TrustworthyWirelessAutoResearch@CUHK SZ** 持有必要权利的原创材料采用 [Creative Commons Attribution 4.0 International License](LICENSE) 授权。使用相关材料时须合理署名、提供许可证链接，并注明是否作出修改。由其他权利或条款约束的材料详见[第三方材料说明](THIRD_PARTY_NOTICES.md)。

建议署名：*Trustworthy Wireless AutoResearch*，**TrustworthyWirelessAutoResearch@CUHK SZ**，2026，[GitHub 仓库](https://github.com/guoyuan-dotcom/TrustworthyWirelessAutoResearch)。

论文级评估流程基于 [WARA](https://github.com/guoyuan-dotcom/WARA_CUHKSZ) 中的 review agent。
