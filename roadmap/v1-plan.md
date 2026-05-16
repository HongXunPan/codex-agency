# Agency 实施计划 v1

本版本目标：

- 建立全局 agency 目录结构与命令入口
- 实现任务分类、角色路由、轻量 prompt bundle
- 记录会话、反馈、候选记忆与审批状态
- 落地方法记忆、领域经验记忆与规避规则
- 将本次规划沉淀为路线图文件与决策日志

当前已完成：

- v2 分层存储、shared/local/project 目录、稳定 project id 与 bootstrap 默认配置
- 语义路由正式落地，已支持 replay 与第一轮调优
- style_trait 指令风格学习闭环、approved 灰度入 prompt、命中调试与健康视图
- review backlog 总盘与审批链路收口，pending / on-hold / backlog 已清零
- status overview / routing / review-backlog / style-trait / learning-guard 等状态视图
- shared repo 同步、maintenance 流程与 project init/show 基础能力

当前剩余：

- 对真实全局数据跑一轮受控 learn 回放，产出 learning_guard 真统计
- 继续做语义路由第二轮调优，降低 fallback 比例
- 给 codex 工作区补 .codex-project.toml，结束 path_fallback / local_only 状态
- 让 style_trait 在真实全局数据里形成 approved 与命中样本
- 补最小回归基线，并继续同步 roadmap 真相

分阶段路径：

1. 骨架与 CLI —— 已完成
2. 角色系统 —— 已完成
3. 反馈抓取 —— 已完成
4. 异步学习 —— 已完成第一阶段，已补 learning guard
5. 审批与长期记忆 —— 已完成当前收口
6. 升级提案与路线图维护 —— 进行中
7. 云同步 —— 已完成基础能力，后续按需要增强
