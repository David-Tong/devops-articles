# 03 - 站点可靠性工程（Site Reliability Engineering）

站点可靠性工程（SRE）将软件工程方法引入运维领域，目标是构建和维护高可靠、可扩展、高效率的生产系统。

## 主题目录

### SRE 基础理念
- SRE 思维模式：错误预算（Error Budget）、减少重复劳动与可靠性目标
- 服务级别指标（SLI）、目标（SLO）与协议（SLA）的定义与实践
- 可靠性工作与功能迭代速度之间的平衡
- 无责文化（Blameless Postmortem）与从故障中学习

### 可观测性（Observability）
- 可观测性三支柱：指标（Metrics）、日志（Logs）、追踪（Traces）
- 指标体系：Prometheus 采集与 Grafana 告警最佳实践
- 结构化日志：设计规范、采集与查询（ELK Stack、Loki）
- 分布式追踪：OpenTelemetry、Jaeger、Tempo
- 监控大盘设计与 Runbook 编写规范

### 故障管理
- On-Call 轮值设计：排班、升级策略与疲劳预防
- 故障响应全流程：发现、响应、止损、恢复、复盘
- 严重等级分类与对外沟通规范
- 真正被使用的 Runbook 与 Playbook 如何编写
- 故障复盘与行动项跟踪机制

### 可靠性设计模式
- 熔断器（Circuit Breaker）、重试与超时
- 舱壁隔离（Bulkhead）与限流（Rate Limiting）
- 优雅降级与兜底策略
- 混沌工程：原则与工具实践（Chaos Monkey、Litmus）

### 容量规划与性能
- 压力测试与基准测试（k6、Locust、JMeter）
- 容量规划模型与需求预测
- 自动扩缩容策略：被动响应 vs 预测式扩容
- 数据库性能调优与慢查询治理

### 减少重复劳动（Toil Reduction）
- 如何识别和量化 Toil
- 运维任务自动化框架设计
- 自愈系统与自动修复机制
- 基于 PagerDuty Runbook Automation 等工具的 Runbook 自动化

### 安全与合规
- 漏洞管理与补丁更新节奏
- 合规即代码：OPA/Gatekeeper、Falco
- 审计日志与访问控制
- 灾难恢复（DR）与业务连续性计划（BCP）
