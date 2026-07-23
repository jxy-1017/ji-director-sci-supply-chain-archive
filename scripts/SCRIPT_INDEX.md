# 代表性脚本索引

仓库不复制原始工作脚本，仅登记用途、状态和隐私边界。

| 脚本 | 用途 | 输入 | 输出 | 实际执行 | 完成 | 验证 | 当前有效性 | TASK | RUN | 可公开 | 绝对路径 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| build_route_b_att_sample_with_g.py | 政策时间与真实G | 企业政策面板 | 处理批次表 | 历史执行 | 完成 | 方法验证 | 历史有效 | TASK-ROUTE-B | historical | 否 | 待脱敏 |
| run_route_b_exploratory_v4_true_g.R | CS-DID真实G技术验证 | 技术样本 | 验证日志 | 已执行 | 完成 | 方法验证 | 可复用 | TASK-ROUTE-B | historical | 否 | 待脱敏 |
| build_route_b_identification_audit.py | 政策单元支持审计 | 政策单元与样本 | 支持报告 | 已执行 | 完成 | 已验证 | 可复用 | TASK-ROUTE-B | historical | 否 | 待脱敏 |
| audit_route_b_source_evidence_v3.py | 结果变量来源审计 | 说明与字段 | 来源报告 | 已执行 | 完成 | 已验证 | 可复用 | TASK-ROUTE-B | historical | 否 | 待脱敏 |
| profile_all_structured_fields_v3_4a.py | 170字段画像 | 结构化字段 | 画像CSV | 已执行 | 完成 | 检查点验证 | 有效 | TASK-ATLAS | RUN-20260723-004 | 否 | 是 |
| audit_and_section_mda_text_v3_4a.py | MD&A编码与章节切分 | TXT索引 | 审计与章节索引 | 已执行 | 完成 | 检查点验证 | 有效 | TASK-ATLAS | RUN-20260723-004 | 否 | 是 |
| audit_factset_terminal_semantics_v3_4a.py | FactSet主键/end终局审计 | 关系工作副本 | 终局摘要 | 已执行 | 完成 | 检查点验证 | 有效 | TASK-ATLAS | RUN-20260723-004 | 否 | 是 |
| certify_factset_working_copy_v3_4a.py | FactSet工作副本认证 | 关系工作副本 | 认证摘要 | 已执行 | 完成 | 检查点验证 | 有效 | TASK-ATLAS | RUN-20260723-004 | 否 | 是 |
| build_fulltext_representations_v3_4a.py | 全文表示 | 章节索引 | NPZ批次 | 部分执行 | 未完成 | 部分输出验证 | 恢复前条件有效 | TASK-V34A | RUN-20260723-004 | 否 | 是 |
| run_topic_ensemble_v3_4a.py | 主题模型 | 完整表示 | 主题输出 | 未执行 | 未完成 | 仅AST | 当前禁止执行 | TASK-V34A | RUN-20260723-004 | 否 | 是 |
| rebuild_semantic_residuals_v3_4a.py | 语义残余重建 | 主题输出 | 残余队列 | 未执行 | 未完成 | 仅AST | 当前禁止执行 | TASK-V34A | RUN-20260723-004 | 否 | 是 |
| finalize_machine_deep_atlas_v3_4a.py | Atlas finalizer | 完整检查点 | 汇总与上传包 | 未执行 | 未完成 | 仅AST | 当前禁止执行 | TASK-V34A | RUN-20260723-004 | 否 | 是 |
