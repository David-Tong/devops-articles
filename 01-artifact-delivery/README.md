# 01 - 制品交付（Artifact Delivery）

制品交付涵盖软件制品的构建、打包、版本管理与分发等全流程工程实践，目标是让每一个可部署的制品都可追溯、可复现、可信赖。

## 文章列表

| 编号 | 文章 | 简介 |
|------|------|------|
| 01 | [软件发布流水线概览](./01-release-pipeline-overview/README.md) | 托管平台视角：PR、主干、Release 三条核心交付流水线的职责与全景 |
| 02 | [非托管环境的容器化交付流水线](./02-container-delivery-pipeline/README.md) | 自建 K8s 环境下，从构建镜像、推送仓库到 Kubernetes 发布的完整流程 |

## 主题目录

### 构建系统
- 主流构建工具对比（Maven、Gradle、Make、Bazel）
- 可复现构建与密封构建环境
- 增量构建与缓存策略
- 单体仓库（Monorepo）与多仓库（Polyrepo）的构建流水线设计

### 持续集成（CI）
- CI 流水线设计原则
- 分支策略与主干开发（Trunk-Based Development）
- Pull Request 质量门禁：代码检查、自动化测试、安全扫描
- CI 性能优化与并行化实践

### 制品打包
- 容器镜像：Dockerfile 最佳实践与多阶段构建
- Helm Chart 与 Kubernetes 清单文件管理
- 各语言包格式（JAR、wheel、npm tarball、NuGet）
- 软件物料清单（SBOM）与制品签名

### 制品仓库
- 主流仓库方案对比：Docker Hub、JFrog Artifactory、AWS ECR、GitHub Packages
- 镜像标签与版本策略（语义化版本、Git SHA、日历版本）
- 制品保留策略与存储成本管理
- 上游仓库代理与缓存配置

### 发布管理
- 语义化版本（SemVer）与变更日志自动化
- 发布分支与 Tag 工作流
- 功能开关（Feature Flag）与暗启动（Dark Launch）
- 回滚策略设计

### 安全与合规
- CI 阶段漏洞扫描工具实践（Trivy、Grype、Snyk）
- 软件供应链安全：SLSA 框架、Sigstore/Cosign 签名
- 开源许可证合规扫描
- 源代码与镜像中的密钥泄露检测
