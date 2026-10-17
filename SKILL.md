---
name: gaoxiang-di4ban-jiaocai
description: "高项（信息系统项目管理师）第4版备考 Skill Pack：24章框架 + 11个教练。覆盖十大管理 ITTO、8个绩效域、挣值/关键路径计算、案例找茬、论文三件套、备考路线与错题归因。当考生问'ITTO/挣值算不对/关键路径不一致/案例不知道找什么/论文没项目/每天只有1小时/总是同类错'时使用；用于备考答疑、框架梳理、出题与术语核对。"
---

<!-- argument-hint: 进度管理 / 绩效域 / 挣值 / 论文 / 案例找错 / 十大管理 / 变更 -->

# 信息系统项目管理师教程（第4版）· 备考框架库
**Author**: 软考办指定教程（高项第4版） | **Pages**: ~700 | **Chapters**: 24 | **Generated**: 2026-10-16

## How to Use This Skill

- **不带参数** — 加载下方核心框架做总体参考
- **带主题** — 说「挣值」「绩效域」「变更流程」等，我定位并读取对应章节
- **带章号** — 说「ch10」，我加载该章文件
- **浏览** — 问「有哪些章节」，看完整索引
- **找教练** — 说「挣值算不对」「案例不知道找什么」「论文没项目」「每天只有1小时」，我加载 `coaches/` 对应模块（不直接给答案，先追问）
- **看技能地图** — 问「怎么用这套 skill」，我读取 `INDEX.md`

> 注意：本 skill 是**框架/原则/技法/反模式层**，不是教材全文。需要逐句原文时，底层 clean 正文在 `D:\WorkBuddy\Claw\高项教材知识库\`（24 章 markdown），本 skill 每条都标注了对应章号，可直接回查。

---

## 教练系统（Coaches · 六段式 R/I/A1/A2/E/B）

> 知识库回答"是什么"，教练回答"你卡在哪、怎么练"。默认**不直接给答案**，先用分层追问暴露空缺。

| 触发 | 教练模块 |
|---|---|
| ITTO / 输入输出 / 哪个过程组 | [01-itto-framework-coach](coaches/01-itto-framework-coach.md) |
| 错题 / 选了A答案是C | [02-mcq-diagnoser](coaches/02-mcq-diagnoser.md) |
| CV/CPI/EAC/ETC 算不对 | [03-evm-step-debugger](coaches/03-evm-step-debugger.md) |
| 关键路径 / 总浮动 / 自由浮动 | [04-cpm-reverse-checker](coaches/04-cpm-reverse-checker.md) |
| 案例不知道从哪找问题 | [05-case-finding-coach](coaches/05-case-finding-coach.md) |
| 论文没项目 / 素材怎么攒 | [06-essay-material-builder](coaches/06-essay-material-builder.md) |
| 论文偏题 / 深度不够 / 结构失衡 | [07-essay-framework-diagnoser](coaches/07-essay-framework-diagnoser.md) |
| 担心被判套作 / 模板化 | [08-essay-anti-template](coaches/08-essay-anti-template.md) |
| 每天1小时 / 还有X个月 | [09-study-route-planner](coaches/09-study-route-planner.md) |
| 每天练一点 / 今天练什么 | [10-daily-drill-scheduler](coaches/10-daily-drill-scheduler.md) |
| 总是同类错 / 错题怎么总结 | [11-mistake-attribution-log](coaches/11-mistake-attribution-log.md) |

**编排原则**：先判"是知识问题还是训练问题"——问定义/框架 → 查 `chapters/`；问"我为什么错/怎么练" → 进教练。教练只做追问与纠错，不代写、不代算、不押题。

---

## Core Frameworks & Mental Models

**1. 双主线结构（第4版最大变化）**
- 传统主线：**十大管理**（第8–17章），每个管理域 = 过程 + 输入/工具与技术/输出（ITTO）。
- 新增强化主线：**8 个绩效域**（第18章），第4版用绩效域替代第3版"项目生命周期管理"等旧框架，是命题新热点，务必优先掌握。
- 关系：**绩效域与十大管理过程相互映射**——答题时"过程组视角"和"绩效域视角"都要能切换。

**2. 价值驱动的项目管理知识体系（第6章）**
- **12 条原则**（第4版新增，常考选择题）：成为勤勉、尊重和关心他人的管家；营造协作的项目团队环境；有效沟通；整合环境动态；展现领导力行为；识别并管理风险与不确定性；优化风险应对；根据环境进行裁剪；善用项目收尾创造价值；保持合规；拥抱适应性与韧性；为实现预期成果赋能。
- 知识领域 = 原则 + 过程组 + 项目生命周期 + 8绩效域 + 价值交付系统。

**3. 十大管理过程数（第4版硬事实，勿错）**
整合7 / 范围6 / 进度6（**估算活动资源已归第13章资源管理**）/ 成本4 / 质量3 / 资源6 / 沟通3 / 风险7 / 采购3 / 干系人4 = **共49个过程**。

**4. 案例命题四步演进（2023下→2026上）**
单点找错 → 双拼融合（两个管理域组合考）→ 绩效域应用诊断 → 计算扩围（EMV/线性规划/博弈/指派进案例）。

**5. 论文四段式（2025起取消摘要）**
背景段 → 过渡段 → 正文段（按过程/绩效域展开，带真实项目实例）→ 结尾段。字数上限 **3500**（2025上起由2500提至3500）。**AI 辅助阅卷（2025起）**：结构混乱、跑题、雷同更易被识别，务必框架清晰、实例具体。

**6. 机考三必练（高项仅上半年5月考，机考）**
选题标记与题号颜色识别；公式编辑器/画图；论文全屏写作与字数统计。

---

## Chapter Index

| # | Title | Key Frameworks |
|---|-------|----------------|
| [ch01](chapters/ch01-xinxi-fazhan.md) | 信息化发展 | 信息/信息化定义、国家信息化6要素、数字中国 |
| [ch02](chapters/ch02-xinxi-jishu.md) | 信息技术发展 | 计算机/网络/存储、物联网云大区块链AI |
| [ch03](chapters/ch03-xinxixitong-zhili.md) | 信息系统治理 | IT治理、IT审计 |
| [ch04](chapters/ch04-xinxixitong-guanli.md) | 信息系统管理 | 管理方法、数据/运维/安全要点 |
| [ch05](chapters/ch05-xinxixitong-gongcheng.md) | 信息系统工程 | 软件工程、数据工程、系统集成、安全工程 |
| [ch06](chapters/ch06-xiangmu-gailun.md) | 项目管理概论 | 价值驱动体系、12原则、8绩效域总览 |
| [ch07](chapters/ch07-xiangmu-lixiang.md) | 项目立项管理 | 建议与立项、可行性研究、评估与决策 |
| [ch08](chapters/ch08-zhenghe.md) | 项目整合管理 | 7过程 ITTO、整体变更控制 |
| [ch09](chapters/ch09-fanwei.md) | 项目范围管理 | 6过程、WBS、确认范围 |
| [ch10](chapters/ch10-jindu.md) | 项目进度管理 | 6过程、关键路径、进度压缩 |
| [ch11](chapters/ch11-chengben.md) | 项目成本管理 | 4过程、挣值 EVM |
| [ch12](chapters/ch12-zhiliang.md) | 项目质量管理 | 3过程、管理质量vs控制质量 |
| [ch13](chapters/ch13-ziyuan.md) | 项目资源管理 | 6过程、估算活动资源归此章 |
| [ch14](chapters/ch14-goutong.md) | 项目沟通管理 | 3过程、沟通模型、互动沟通 |
| [ch15](chapters/ch15-fengxian.md) | 项目风险管理 | 7过程、定性/定量、应急计划 |
| [ch16](chapters/ch16-caigou.md) | 项目采购管理 | 3过程、合同类型、控制采购 |
| [ch17](chapters/ch17-ganxishiren.md) | 项目干系人管理 | 4过程、权力/利益方格 |
| [ch18](chapters/ch18-jixiaoyu.md) | 项目绩效域 | 8个绩效域、与过程映射 |
| [ch19](chapters/ch19-peizhi-biangeng.md) | 配置与变更管理 | 配置库、变更流程 |
| [ch20](chapters/ch20-gaoji.md) | 高级项目管理 | 项目组合/集、量化项目管理 |
| [ch21](chapters/ch21-kexue-jichu.md) | 项目管理科学基础 | 工程经济、网络计划、运筹（博弈/指派） |
| [ch22](chapters/ch22-zuzhi-zhili.md) | 组织通用治理 | 治理框架、度量体系 |
| [ch23](chapters/ch23-zuzhi-guanli.md) | 组织通用管理 | 营销、人力、财务、行政 |
| [ch24](chapters/ch24-falv-biaozhun.md) | 法律法规与标准规范 | 招投标、政府采购、合同法、著作权 |

## Topic Index

- **挣值/EVM** → ch11, ch21
- **关键路径/进度压缩** → ch10
- **8个绩效域** → ch18, ch06
- **12原则** → ch06
- **变更控制** → ch08, ch19
- **合同类型** → ch16
- **风险应对/应急计划** → ch15
- **WBS** → ch09
- **论文写法** → cheatsheet, patterns
- **案例找错** → patterns
- **计算（EMV/线性规划/博弈/指派）** → ch21

## 常见坑（Gotchas · 最高信号）

1. **进度管理只有 6 个过程**：估算活动资源归第 13 章资源管理，别算进进度。
2. **管理质量 ≠ 控制质量**：前者管过程（审计、设计评审），后者管结果（测试、抽检）。
3. **三类绩效别混**：工作绩效数据（原始）→ 工作绩效信息（对比基准）→ 工作绩效报告（汇总）。
4. **典型/非典型**：题目没说"剩余按原计划"，一律按典型偏差（EAC=BAC/CPI）。
5. **第4版旧词陷阱**：风险监控→**监督风险**；建设项目团队→**建设团队**；交互式沟通→**互动沟通**；人力资源计划→**资源管理计划**；实施质量保证→**管理质量**。
6. **论文不写摘要**，≤3500 字，必须有真实项目与量化成效。
7. **变更不由发起人直接改**：任何变更都要书面请求 → CCB 审批 → 更新基准 → 通知干系人。
8. **配置三库**：开发库 / 受控库 / 产品库；基线产品入受控库。

## Supporting Files

- [INDEX.md](INDEX.md) — 技能地图、使用顺序与触发速查
- [coaches/](coaches/) — 11 个教练模块（六段式 R/I/A1/A2/E/B）
- [examples/](examples/) — 3 个"输入→输出"示例（ITTO / 案例 / 论文）
- [glossary.md](glossary.md) — 核心术语与定义（标注章号）
- [patterns.md](patterns.md) — 案例找错反模式、论文高分技法、计算提速套路
- [cheatsheet.md](cheatsheet.md) — 公式速查、过程清单、决策规则
- [CHANGELOG.md](CHANGELOG.md) — 版本更新记录
- [LICENSE](LICENSE) — CC BY-NC-SA 4.0

---

## Scope & Limits

覆盖高项第4版教程 24 章框架内容 + 11 个教练模块，面向下一轮上半年（5 月）备考（2024 年起高项仅上半年开考）。不含系规/中项内容，不含实时考情公告（以软考办官方为准）。不代写论文、不代算整题、不押题。底层逐句原文见 `D:\WorkBuddy\Claw\高项教材知识库\`。
