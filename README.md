# 火山知识库 - Monorepo项目

![火山知识库](./apps/docs/public/img/logo.png)

这是一个基于Monorepo架构的项目，主要包含火山知识库及其相关应用。目前已开发的应用是基于VitePress构建的技术文档站点。

## 🚀 项目概述

这是一个个人维护的技术学习与分享平台，记录了我在学习和工作过程中的心得体会与技术总结。本项目采用Monorepo架构，便于管理多个相关应用，提高代码复用率，并保持统一的开发体验。

## 🔍 项目结构

```
hs-knowledge-base/
├── apps/                 # 应用目录
│   └── docs/             # 知识库文档应用(VitePress)
│       ├── .vitepress/   # VitePress配置和主题
│       ├── public/       # 静态资源
│       ├── client/       # 客户端技术内容
│       │   ├── web前端技术/       # Web开发相关技术
│       │   ├── 移动应用技术/      # React Native、Flutter、小程序等
│       │   ├── 桌面应用技术/      # Electron、Tauri等跨平台桌面技术
│       │   ├── 3D与可视化技术/    # Three.js、WebGL、数据可视化等
│       │   ├── 测试与质量保障/    # 前端测试、性能优化、兼容性等
│       │   └── 工程化与最佳实践/  # 工程架构、CI/CD、设计系统等
│       ├── server/       # 服务端技术内容
│       │   ├── 开发语言与框架/   # 各类编程语言及框架
│       │   ├── 数据存储技术/     # 数据库与缓存系统
│       │   ├── 中间件技术/       # 消息队列、API网关等
│       │   ├── 架构与设计模式/   # 微服务、DDD等架构
│       │   ├── 运维与部署/       # 服务端应用部署与运维
│       │   └── 安全技术/         # 认证授权、加密等
│       ├── systems/      # 系统与底层内容
│       │   ├── 系统编程语言/     # Rust等系统编程语言
│       │   ├── 操作系统与内核/   # 操作系统原理、内核与驱动开发
│       │   ├── 性能优化与调优/   # 算法优化、并行计算、性能分析
│       │   ├── 编译与运行时/     # 编译原理、JIT、垃圾回收、虚拟机
│       │   └── 跨平台技术/       # WebAssembly、跨平台工具链等
│       ├── devops/       # DevOps与云原生内容
│       │   ├── 持续集成与交付/    # CI/CD、自动化测试、部署策略等
│       │   ├── 容器与编排/        # Docker、Kubernetes、服务网格等
│       │   ├── 监控与可观测性/    # 指标、日志、追踪、告警等
│       │   ├── 基础设施即代码/    # Terraform、配置管理、GitOps等
│       │   └── 安全与合规/        # DevSecOps、容器安全、合规自动化等
│       ├── ai/           # AI应用与大模型内容
│       │   ├── 基础模型技术/     # LLM、多模态模型等基础模型
│       │   ├── 开发与工程化/     # Prompt工程、开发框架等
│       │   ├── 应用与集成/       # Agents、RAG、架构设计等
│       │   ├── 部署与优化/       # 模型部署、性能优化等
│       │   └── 安全与伦理/       # AI安全、伦理与合规等
│       ├── packages/             # 共享包目录(待开发)
│       ├── package.json          # 根项目配置
│       └── pnpm-workspace.yaml   # Monorepo工作区配置
```

## ⚙️ 开发指南

### 环境准备

```bash
# 安装 pnpm（如果尚未安装）
npm install -g pnpm

# 安装所有依赖
pnpm install
```

### 常用命令

```bash
# 启动知识库开发服务器
pnpm docs:dev

# 构建知识库生产版本
pnpm docs:build

# 预览知识库构建结果
pnpm docs:preview
```

## 📚 已实现应用

### 火山知识库 (apps/docs)

这是一个技术文档站点，内容涵盖以下技术领域：

- **客户端技术**：
  - Web前端技术：HTML/CSS/JavaScript、现代框架、构建工具、Web API等
  - 移动应用技术：React Native、Flutter、小程序等跨平台解决方案
  - 桌面应用技术：Electron、Tauri等跨平台桌面技术
  - 3D与可视化技术：Three.js、WebGL、数据可视化等
  - 测试与质量保障：单元测试、E2E测试、性能测试、兼容性测试等
  - 工程化与最佳实践：工程架构、CI/CD、设计系统、安全实践等
- **服务端技术**：
  - 开发语言与框架：Node.js、Go、Java、Python等语言及其框架
  - 数据存储技术：关系型数据库、NoSQL、内存数据库、时序数据库等
  - 中间件技术：消息队列、缓存系统、API网关、服务发现等
  - 架构与设计模式：微服务架构、DDD、事件驱动架构等
  - 运维与部署：从服务端开发者视角的应用部署与运维
  - 安全技术：认证授权、数据加密、安全最佳实践等
- **系统与底层**：
  - 系统编程语言：Rust、Go系统编程、语言互操作等
  - 操作系统与内核：操作系统原理、内核开发、驱动、虚拟化等
  - 性能优化与调优：算法优化、编译器优化、并行计算、性能分析等
  - 编译与运行时：编译原理、JIT、垃圾回收、虚拟机与解释器等
  - 跨平台技术：WebAssembly、跨平台工具链、抽象层设计等
- **DevOps与云原生**：
  - 持续集成与交付：CI/CD、自动化测试、部署策略等
  - 容器与编排：Docker、Kubernetes、Helm、服务网格等
  - 监控与可观测性：Prometheus、Grafana、ELK、分布式追踪等
  - 基础设施即代码：Terraform、Ansible、GitOps工作流等
  - 安全与合规：DevSecOps、容器安全、合规自动化等
- **AI应用与大模型**：
  - 基础模型技术：LLM、多模态模型、预训练技术等
  - 开发与工程化：Prompt工程、开发框架、工程最佳实践等
  - 应用与集成：AI Agents、RAG、架构设计、行业应用等
  - 部署与优化：模型部署、量化优化、推理加速等
  - 安全与伦理：AI安全、隐私保护、伦理与合规等

#### 特色功能

- 响应式设计，适配各种设备
- 深色/浅色主题切换
- 自动生成侧边栏导航
- 全文检索功能

## 🔄 Monorepo优势

- **代码共享**：可在不同应用间共享组件和工具
- **统一开发体验**：所有项目使用相同的工具链和规范
- **原子化提交**：关联变更可在单次提交中完成
- **集中依赖管理**：减少冗余依赖，简化更新

## 🛣️ 项目规划

1. **已完成**：火山知识库文档站点(VitePress)
2. **规划中**：
   - 知识图谱可视化工具
   - 代码示例展示平台
   - API文档生成工具

## 🤝 参与贡献

我欢迎各种形式的贡献，包括内容修正、新功能开发和应用创意。你可以通过以下方式参与：

- 提交Issue或Pull Request
- 通过邮件联系我提供反馈
- 分享这个项目给更多需要的人

## 📄 许可证

MIT 