# OpenCode iOS 开发 Agent 合集

39 个中文 OpenCode 子代理，覆盖 iOS 越狱插件和 App 开发全流程。

## 安装

```bash
mkdir -p ~/.config/opencode/agents
git clone https://github.com/ac54u/agent.git /tmp/agent
cp /tmp/agent/*.md ~/.config/opencode/agents/
rm -rf /tmp/agent
```

重启 opencode 后 `@名称` 调用。

---

## 🔧 工程开发 (15)

### `@mobile-app-builder` 移动应用构建器
```
@mobile-app-builder 这个 SwiftUI 列表视图性能怎么优化，目前滚动掉帧
@mobile-app-builder 帮我设计一个音频变声功能的架构方案，用 AVFoundation
@mobile-app-builder iOS 16+ 的 SwiftUI NavigationStack 怎么替代 NavigationView
@mobile-app-builder 这个 Objective-C 代码怎么迁移到 Swift，注意 ARC 兼容
@mobile-app-builder iPhone 和 iPad 双端适配的最佳实践是什么
@mobile-app-builder 评估一下原生 iOS vs React Native vs Flutter 选型，我们这个项目是越狱插件
```

### `@voice-ai-integration-engineer` 语音 AI 集成工程师
```
@voice-ai-integration-engineer 用 AVFoundation 做实时语音采集 + 变声处理，给个完整方案
@voice-ai-integration-engineer 离线 Whisper 模型在 iOS 上怎么部署，性能如何
@voice-ai-integration-engineer 音频流实时转文字的最佳管道设计，AAC → PCM → 特征提取
@voice-ai-integration-engineer 语音文件格式检测：怎么用 magic bytes 识别 AAC/M4A/MP3/WAV
@voice-ai-integration-engineer 变声后音频拉伸/失真怎么处理？重采样到 48000Hz 是不是必须的
@voice-ai-integration-engineer 语音评论抓取场景：从缓存提取音频 + 变声 + 重新编码给个端到端方案
```

### `@rapid-prototyper` 快速原型开发师
```
@rapid-prototyper 2 小时内搭一个 Tweak 弹窗选择器的 MVP，Theos + Objective-C
@rapid-prototyper 快速验证 DYYY 语音变声功能是否可行，忽略边界情况
@rapid-prototyper 这个 Hook 点子行不行？对 Aweme 的评论输入框注入自定义菜单
@rapid-prototyper 搭一个简单的 iOS 设置页面 POC，要点击切开关、滑动选值、弹确认框
```

### `@codebase-onboarding-engineer` 代码库入门工程师
```
@codebase-onboarding-engineer 帮我理解 Aweme 的音频播放链，从用户点击到 AVAudioPlayerNode 的完整调用路径
@codebase-onboarding-engineer DYYYManager.m 的 dispatch_queue 架构是怎样的，帮我画个调用图
@codebase-onboarding-engineer 这个 ObjC Tweak 项目入口在哪，Hook 是怎么注入的，讲清楚 %hook 机制
@codebase-onboarding-engineer 追踪一下语音评论下载后保存路径，相关文件有哪些
```

### `@code-reviewer` 代码审查员
```
@code-reviewer 审查 DYYYVoiceChanger.m 的改动，重点关注内存管理和线程安全
@code-reviewer 这段音频转码代码有潜在 crash 吗？帮我做安全审查
@code-reviewer 审查这个 PR：AVAssetWriter 使用是否正确，CMSampleBuffer 生命周期对不对
@code-reviewer 这段 dispatch_semaphore 用法有没有死锁风险
@code-reviewer 检查 DYYYManager.m 单例模式是否有线程安全问题
```

### `@minimal-change-engineer` 最小变更工程师
```
@minimal-change-engineer DYYYVoiceChanger crash：只修复 SIGABRT，不要重构其他代码
@minimal-change-engineer 修复这个 if 条件判断的 bug，只改一行，不改变量名和注释
@minimal-change-engineer 给 DYYYManager 加一个开关属性，别碰现有的城市过滤和音频逻辑
@minimal-change-engineer 把这两个 NSLog 改成条件编译输出，仅此而已
```

### `@software-architect` 软件架构师
```
@software-architect 设计 DYYY 越狱插件整体架构：Hook 层 → 管理层 → UI 层 → 音频引擎
@software-architect 音频变声功能怎么分层设计？AVAssetReader → 效果链 → AVAssetWriter
@software-architect 我的 Tweak 有 60 多个 .m 文件，建议怎么模块化拆分和分层
@software-architect 评估当前架构：所有逻辑都在 DYYYManager 单例里，有什么问题怎么重构
```

### `@backend-architect` 后端架构师
```
@backend-architect 设计一个简单的 API 后端，用于接收 iOS 插件上报的音频配置和统计
@backend-architect 变声预设配置的云端存储方案：RESTful API 设计 + SQLite/PostgreSQL 选型
@backend-architect 语音文件上传的断点续传 API 怎么设计
```

### `@ai-engineer` AI 工程师
```
@ai-engineer 在 iOS 上如何部署一个轻量级的语音分类模型，用 CoreML
@ai-engineer 评估 Whisper 在 iPhone 13 上的推理性能，给出部署建议
@ai-engineer 音频特征提取 + 实时分类的端侧机器学习方案
@ai-engineer CoreML 模型怎么从 PyTorch 转换，模型量化到多少 bit 不影响精度
```

### `@frontend-developer` 前端开发者
```
@frontend-developer 帮这个 iOS Tweak 的设置页面用 React Native 实现一个替代方案
@frontend-developer 这个 React Native FlatList 滚动卡顿怎么优化
@frontend-developer TypeScript 类型定义：给 DYYY 配置对象写一个完整的 interface
@frontend-developer Tailwind CSS 实现一个仿 iOS Settings 风格的暗色主题配置页
```

### `@git-workflow-master` Git 工作流大师
```
@git-workflow-master 整理最近 5 个 commit：rebase squash 成 2 个有意义的提交
@git-workflow-master 我的分支策略合适吗？main 直接提交 Tweak 发布版，需不需要 develop 分支
@git-workflow-master 这个 feat/bug/v2 的分支命名规范怎么优化，给个 convention
@git-workflow-master CI 合并失败了，帮我用 git bisect 找到哪个 commit 引入了问题
@git-workflow-master 不小心在 main 上直接改了，怎么撤回但不丢失修改
```

### `@devops-automator` DevOps 自动化专家
```
@devops-automator 优化我的 GitHub Actions 构建流程：Theos 编译 + ar/strip + ldid 签名 + 打包 deb
@devops-automator CI 里怎么缓存 Theos 和 SDK 依赖，每次 clone 太慢了
@devops-automator 设计一个多 scheme 构建流水线：rootless + roothide 并行打包
@devops-automator GitHub Actions 怎么实现自动化 release 发布，上传 deb 到 Release Assets
```

### `@incident-response-commander` 事件响应指挥官
```
@incident-response-commander DYYY 用户反馈安装后 Aweme 闪退，写一份事故复盘模板
@incident-response-commander 排查这个 AVAssetWriter SIGABRT crash：给个分步调查 checklist
@incident-response-commander 建立 Tweak 发布前的质量门禁：什么情况下不能发布
@incident-response-commander 用户反馈声音变声后音量变小，怎么定位是哪个版本引入的
```

### `@mcp-builder` MCP 构建器
```
@mcp-builder 写一个 OpenCode MCP 服务器：自动编译 Theos Tweak 并推送 deb 到设备
@mcp-builder 构建一个 MCP 工具，能读取 Aweme 的可执行文件和链接库列表
@mcp-builder 设计一个 MCP server 让 AI 助手能直接执行 otool/class-dump 命令
```

### `@agents-orchestrator` 智能体编排器
```
@agents-orchestrator 组织一次 DYYY 完整功能开发：需求 → 设计 → 实现 → 审查 → 测试 → 发布
@agents-orchestrator 协调多个 Agent：mobile-app-builder 设计架构 + security-architect 审查 + code-reviewer 复核
```

---

## 📱 产品与市场 (6)

### `@product-manager` 产品经理
```
@product-manager 帮我写一份 DYYY 语音变声插件的产品需求文档 PRD
@product-manager 这个"评论区语音抓取"功能怎么做用户故事拆分和优先级排序
@product-manager 评估下一个版本应该优先做哪个功能：变速播放 vs 环境音消除 vs AI 变声
@product-manager 设计一个功能上线后的用户满意度指标和数据埋点方案
```

### `@senior-project-manager` 高级项目经理
```
@senior-project-manager 把 DYYY v2.0 拆成可执行的开发任务，估算工时，排优先级
@senior-project-manager 当前有 5 个 feature、3 个 bug、2 个优化，帮我排 Sprint
@senior-project-manager 跟踪上次 post-mortem 的改进项，哪个还没完成
```

### `@app-store-optimizer` 应用商店优化师
```
@app-store-optimizer 帮我写 App Store 的应用描述，突出变声和语音处理功能
@app-store-optimizer 分析竞品的关键词策略："变声器""语音特效""音效"这些词怎么布局
@app-store-optimizer 给 DYYY 写 5 组 A/B 测试用的应用截图文案
@app-store-optimizer 中国区 App Store 关键词优化和标题怎么写，ASO 最佳实践
```

### `@china-market-localization-strategist` 中国市场本地化策略师
```
@china-market-localization-strategist DYYY 怎么在抖音/小红书做推广，目标用户是 Aweme 用户
@china-market-localization-strategist 这个插件的中文命名和功能描述怎么接地气又不违规
@china-market-localization-strategist 分析一下 Aweme 用户画像，我们的功能定位对不对
```

### `@trend-researcher` 趋势研究员
```
@trend-researcher iOS 越狱社区 2024-2025 趋势：哪些类型的 Tweak 需求在增长
@trend-researcher AI 语音合成/SVC 在移动端的应用趋势，DYYY 怎么卡位
@trend-researcher 竞品分析：市面上主流的语音变声 App 都做了什么功能，我们缺什么
```

### `@developer-advocate` 开发者布道师
```
@developer-advocate 帮我写 DYYY 的技术博客：如何 Hook Aweme 的音频引擎实现实时变声
@developer-advocate 写一份 DYYY 插件接入文档，让其他开发者能二次开发
@developer-advocate GitHub README 怎么写能吸引更多 Star 和贡献者
```

---

## 🎨 设计 (2)

### `@ui-designer` UI 设计师
```
@ui-designer 设计 DYYY 变声设置界面：滑块 + 预设选择 + 实时预览波形
@ui-designer 给 DYYY 做一套 iOS 风格的暗色主题设计规范
@ui-designer 变声确认弹窗的交互设计：怎么提示用户处理完成，Toast 还是 Alert
```

### `@ux-researcher` UX 研究员
```
@ux-researcher 用户访谈脚本：了解用户对变声功能的核心诉求和痛点
@ux-researcher 设计一个 A/B 测试：弹窗确认 vs 自动处理，哪种体验更好
@ux-researcher 分析 DYYY 的用户操作流程有没有卡点，怎么优化到最少点击
```

---

## 🧪 测试与质量 (7)

### `@reality-checker` 现实检验官
```
@reality-checker DYYY 这个版本能发布吗？做一次完整的部署就绪审查
@reality-checker 检查这次 crash 修复的质量，需要什么额外证据才能认证通过
@reality-checker 审查所有已完成的修改，逐一验证是否真正解决了问题
```

### `@evidence-collector` 证据收集器
```
@evidence-collector 对新 UI 弹窗做截图 QA：深色/浅色模式、中文/英文、iPhone/SE
@evidence-collector 变声前后音频对比：收集频谱图、波形图、播放时长等视觉证据
@evidence-collector 测试 DYYY 与 Aweme 的交互，收集界面变化前后的截图对比
```

### `@performance-benchmarker` 性能基准测试
```
@performance-benchmarker 测量变声处理耗时：30s 音频用 AVAssetReader 走一遍要多久
@performance-benchmarker 对比 busy-wait vs requestMediaDataWhenReadyOnQueue 的性能差异
@performance-benchmarker DYYY 注入后 Aweme 启动时间增加多少，内存多占用多少
@performance-benchmarker 测试不同音频时长（5s/15s/30s/60s）的处理延迟曲线
```

### `@api-tester` API 测试员
```
@api-tester 测试 DYYY 配置下发接口：边界值、并发请求、超时处理
@api-tester AVAssetReader/Writer 的各种输入格式测试：M4A/MP3/WAV/AAC 兼容性矩阵
@api-tester 生成变声功能的 API 测试用例：输入 → 处理 → 输出，验证完整性
```

### `@test-results-analyzer` 测试结果分析师
```
@test-results-analyzer 汇总 DYYY 测试结果：性能/兼容性/crash 率，生成质量报告
@test-results-analyzer 分析最近 10 次 CI 构建的测试数据，趋势是变好还是变差
@test-results-analyzer 变声音质主观评分数据怎么量化分析
```

### `@accessibility-auditor` 无障碍审计员
```
@accessibility-auditor 审计 DYYY 设置页面的无障碍体验：VoiceOver 能否正常朗读所有控件
@accessibility-auditor 检查 UI 控件的 contrast ratio 和 touch target size 是否符合规范
```

### `@model-qa-specialist` 模型 QA 专家
```
@model-qa-specialist 审计变声效果链的音频处理模型：输入输出一致性、延迟稳定性
@model-qa-specialist CoreML 语音模型的精度验证和推理性能 benchmark
```

---

## 🔒 安全 (6)

### `@security-architect` 安全架构师
```
@security-architect DYYY 插件系统有安全风险吗？威胁建模分析：Hook 注入 + 文件读写 + 网络
@security-architect 审查变声音频文件的存储路径和权限，有没有信息泄露风险
@security-architect Hook 第三方 App 的安全性评估：会不会触发反作弊检测
```

### `@application-security-engineer` 应用安全工程师
```
@application-security-engineer 对 DYYY 源码做 SAST 分析：Objective-C 内存安全漏洞扫描
@application-security-engineer 审查 DYYYManager 的沙箱逃逸和文件读写权限
@application-security-engineer 建立 DYYY 的安全开发流程：每次 PR 必过的安全检查项
```

### `@penetration-tester` 渗透测试员
```
@penetration-tester 对 DYYY 做渗透测试：能通过插件获取 Aweme 的用户数据吗
@penetration-tester 测试变声功能的攻击面：恶意音频文件能否触发缓冲区溢出
@penetration-tester 验证 Tweak 注入点的安全性：Cydia Substrate Hook 是否可被其他插件污染
```

### `@incident-responder` 事件响应员
```
@incident-responder DYYY 用户反馈插件导致 Aweme 账号被封，怎么做 DFIR 溯源
@incident-responder 音频文件被恶意替换导致 crash，做一次完整的入侵调查分析
@incident-responder 建立 DYYY 安全事件的应急响应手册和联系人清单
```

### `@compliance-auditor` 合规审计员
```
@compliance-auditor DYYY 处理用户音频数据是否符合 Apple 隐私政策和 GDPR 要求
@compliance-auditor 审计变声功能的合规性：音频处理是否涉及用户内容审核风险
@compliance-auditor App Store 审核指南对照检查：DYYY 会不会被判定为违规插件
```

### `@cloud-security-architect` 云安全架构师
```
@cloud-security-architect DYYY 的配置下发服务器怎么做零信任架构设计
@cloud-security-architect 变声预设同步到 iCloud 的安全方案：端到端加密 + keychain
```

---

## 🔧 工具与流程 (3)

### `@tool-evaluator` 工具评估员
```
@tool-evaluator 评估 iOS 音频处理框架选型：AVAudioEngine vs AudioUnit vs The Amazing Audio Engine
@tool-evaluator 对比几个越狱开发工具链：Theos vs iOSOpenDev vs DragonBuild
@tool-evaluator 评估崩溃收集工具：Crashlytics vs Sentry vs 自建方案
```

### `@workflow-optimizer` 工作流优化员
```
@workflow-optimizer 优化 DYYY 的开发-测试-发布流程：改代码 → 编译 → SSH 推送到真机
@workflow-optimizer CI 构建太慢（8分钟），分析瓶颈在哪，怎么优化到 3 分钟
@workflow-optimizer 建立 Code Review 的标准流程和检查清单
```

### `@technical-writer` 技术文档撰写者
```
@technical-writer 给 DYYY 写一份完整的 README：功能说明、安装方法、开发指南、FAQ
@technical-writer 写一篇技术博客：我是如何 Hook Aweme 音频引擎的
@technical-writer 把 DYYY 的 API 注释整理成规范的文档，补全参数说明和返回值
```

---

## 组合用法

多 Agent 协同工作：

```
# 代码审查流程
@code-reviewer 审查 DYYYVoiceChanger.m
然后 @reality-checker 这个 PR 能合吗

# 功能开发流程
@software-architect 设计变声功能的分层架构
然后 @mobile-app-builder 实现核心组件
然后 @performance-benchmarker 测试处理延迟
然后 @code-reviewer 审查全部代码

# 发布流程
@evidence-collector 截图验证 UI 正常
@performance-benchmarker 确认性能无回归
@reality-checker 认证可以发布
@git-workflow-master 整理 commit 打 tag
@devops-automator 触发 CI 发版
```
