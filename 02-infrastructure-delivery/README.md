# 02 - 基础设施交付（Infrastructure Delivery）

基础设施交付涵盖以代码方式定义、配置和管理基础设施的工程实践，目标是让每一套环境都可版本化、可审计、可一键重建。

## 主题目录

### 基础设施即代码（IaC）
- Terraform 核心概念：Provider、State、Module 与 Workspace
- Pulumi 与 CDK 作为 HCL 的替代方案
- State 管理：远程后端、锁机制与漂移（Drift）检测
- IaC 测试实践：Terratest、Checkov、tfsec

### 配置管理
- Ansible：Playbook、Role 与 Inventory 管理
- 声明式配置与命令式配置的对比与选择
- 密钥注入方案：Vault、AWS Secrets Manager、Azure Key Vault
- 不可变基础设施模式

### 云平台
- AWS 核心服务在交付流水线中的应用（EC2、ECS、EKS、Lambda、CodePipeline）
- Azure DevOps 与 Azure 基础设施实践
- GCP 基础设施与 Cloud Build
- 多云与混合云架构考量

### Kubernetes 与容器编排
- 集群生命周期管理与版本升级
- 命名空间策略与多租户隔离
- 资源管理：Request/Limit 与自动扩缩容（HPA、VPA、KEDA）
- GitOps 实践：Flux 与 Argo CD

### 网络与安全
- VPC 设计、子网划分与网络策略
- 服务网格：Istio 与 Linkerd
- Ingress 控制器与 API 网关
- IAM 最佳实践与最小权限原则

### 持续交付（CD）
- 部署策略：滚动更新、蓝绿部署、金丝雀发布
- 渐进式交付与功能开关
- 流水线即代码：GitHub Actions、GitLab CI、Jenkins
- 环境晋级（Environment Promotion）工作流

### 成本管理
- FinOps 基础：资源标签、成本归属（Showback）与费用分摊（Chargeback）
- 计算资源合理化与预留容量规划
- Spot/抢占式实例使用策略
- 基础设施成本预测与预警
