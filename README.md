# OpenCode iOS 开发 Agent 合集

22 个中文 OpenCode 子代理，覆盖 iOS 越狱插件和 App 开发全流程。

## 安装

```bash
# 全局安装
mkdir -p ~/.config/opencode/agents
git clone https://github.com/ac54u/agent.git /tmp/agent
cp /tmp/agent/*.md ~/.config/opencode/agents/
rm -rf /tmp/agent
```

重启 opencode 后 `@名称` 调用。

## Agent 列表

### 🔧 工程开发
| Agent | 用途 |
|---|---|
| `@mobile-app-builder` | iOS/Android 原生 + 跨平台开发 |
| `@voice-ai-integration-engineer` | Whisper 语音转录/AI 音频 |
| `@rapid-prototyper` | POC/MVP 快速验证 |
| `@codebase-onboarding-engineer` | 阅读源码、追踪调用链 |
| `@code-reviewer` | 代码审查：正确性、安全、性能 |
| `@minimal-change-engineer` | 最小 diff，拒绝范围蔓延 |
| `@software-architect` | 系统设计、DDD、架构模式 |
| `@backend-architect` | API 设计、数据库、微服务 |
| `@ai-engineer` | CoreML / ML 模型集成 |
| `@git-workflow-master` | 分支策略、约定式提交 |
| `@devops-automator` | CI/CD、云运维 |
| `@incident-response-commander` | 生产事故应急、复盘 |

### 🔒 安全
| Agent | 用途 |
|---|---|
| `@security-architect` | 威胁建模、纵深防御 |
| `@penetration-tester` | 渗透测试、漏洞评估 |

### 🧪 测试与质量
| Agent | 用途 |
|---|---|
| `@reality-checker` | 证据驱动上线认证 |
| `@evidence-collector` | 截图 QA、视觉证据 |
| `@performance-benchmarker` | 性能基准测试 |
| `@api-tester` | API 自动化测试 |
| `@test-results-analyzer` | 测试结果分析 |
| `@accessibility-auditor` | 无障碍审计 |

### 🔧 工具与流程
| Agent | 用途 |
|---|---|
| `@tool-evaluator` | 框架/工具技术选型 |
| `@workflow-optimizer` | 开发流程分析与优化 |

## 使用方式

```
@code-reviewer 审查这段 ObjC 代码
@mobile-app-builder 这个 SwiftUI 视图怎么优化
@reality-checker 检查改动质量
@voice-ai-integration-engineer 音频格式转换
@minimal-change-engineer 修复这个 crash
```
