# 供应链论文项目：过程归档与GitHub时间线

本私有仓库记录项目自2026年3月启动至2026年7月23日的研究过程，包括数据范围与质量审计、候选路线变化、方法验证、路线终止依据、脚本与运行索引、阶段汇报和工作交接。

本仓库不是原始数据库备份、商业数据库公开仓库、全文语料仓库或已完成论文结果仓库。当前尚未冻结正式论文主线，除数据和方法审计事实外，不对政策效果或企业结果作正式结论。

## 当前状态

- 路线B已经开展探索性和技术验证估计，但在进入正式论文主规格、正式结果解释和论文写作之前终止。状态为 `TERMINATED_DO_NOT_REVIVE`；终止依据是结果变量来源、底层字段、数据库coverage和政策单元支持不足，不是因为统计显著性。
- 四个数据域的机器级全量清点已完成；Atlas V3.4A机器深度任务尚未完成。
- V3.4A七类全文表示连续存在第1—76批，第77—92批缺失；当前状态为 `PROJECT_ALL_DATA_ATLAS_MACHINE_DEEP_INCOMPLETE_AT_CHECKPOINT`。
- 主题模型、语义残余重建和finalizer均未执行，`CHAT_UPLOAD_PACK`不存在。
- 恢复状态为 `SAFE_RESUME_CONDITIONAL_ON_TARGETED_NPZ_LOAD_TEST`，不得直接升级为无条件续跑。

详细证据见[运行记录](runs/2026-07/RUN-20260723-004-v34a-interrupted/RUN_RECORD.md)、[实际进度](runs/2026-07/RUN-20260723-004-v34a-interrupted/ACTUAL_PROGRESS.md)和[安全恢复边界](runs/2026-07/RUN-20260723-004-v34a-interrupted/SAFE_RESUME_BOUNDARY.md)。

## 研究执行说明

项目负责人负责研究问题定义、数据范围、分析规则、识别边界、脚本需求、运行检查、结果核验和路线决策。项目中形成并维护了数据清洗、字段审计、实体映射和模型验证脚本，并根据数据结构、报错和审计结果持续修订；编程和自动化辅助工具用于提高大规模处理效率。

## 仓库结构

- `docs/`：项目、时间线、路线、方法和Atlas说明。
- `weekly_logs/`：依据现有材料进行的阶段性事后重建。
- `tasks/`：计划任务索引；TASK表示计划做什么。
- `runs/`：实际运行记录；RUN表示实际做了什么。
- `checkpoints/`：检查点摘要索引，不保存完整机器工作区。
- `scripts/`：代表性脚本登记和使用状态，不复制敏感或商业数据脚本。
- `data_registry/`：不可入库数据资产的脱敏登记。
- `evidence/`：方法、决策和来源证据索引。
- `briefings/`：面向项目负责人、合作教师和接手研究人员的阶段汇报。

## 数据不可公开

FactSet/Revere、GSDB、企业面板和MD&A全文受授权、隐私、体积或商业数据库限制，不进入Git。仓库仅保存脱敏元数据、检查点摘要、证据链和小型审计结果。

## 当前下一步

人工审核本归档；如后续恢复V3.4A，应先在已有scipy环境中执行指定NPZ只读抽检，抽检通过后才从第77批恢复全文表示。新论文方向仍需在数据映射与识别支持审计后认证。

## 重要入口

- [当前状态](CURRENT_STATUS.md)
- [项目时间线](PROJECT_TIMELINE.md)
- [决策日志](DECISION_LOG.md)
- [路线B终止记录](docs/routes/route_b/ROUTE_B_TERMINATION_RECORD.md)
- [数据Atlas历史](docs/data_atlas/DATA_ATLAS_HISTORY.md)
- [V3.4A当前状态](docs/data_atlas/V3_4A_CURRENT_STATE.md)
- [2026-07-23阶段汇报](briefings/2026-07-23/PROJECT_STATUS_ONE_PAGE.md)
