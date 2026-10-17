# 更新日志

遵循 [语义化版本](https://semver.org/lang/zh-CN/)。

## [0.3.1] - 2026-10-17

### 修正
- **12 条原则**改为第 4 版官方口径。原列表有 6 处错误（"有效沟通""整合环境动态""善用项目收尾创造价值""保持合规""识别并管理风险与不确定性"重复计入风险、"为实现预期成果赋能"），现按教材第 6 章更正。
- `coaches/` 下 `test-prompts.json` 所在目录与同名 `.md` 文件冲突 → 统一移至 `coaches/tests/`。
- `LICENSE` 换为 CC BY-NC-SA 4.0 官方全文（GitHub 可正确识别，原为 `NOASSERTION`）。

## [0.3.0] - 2026-10-17

### 变更
- 11 个教练升级为完整版：补充"博主经验分布"、完整算例、2–4 个反例、5 层追问脚本、使用示例。
- 新增 3 个核心教练的 `test-prompts.json`（evm / cpm / case-finding）。
- `INDEX.md` 增加"三科 × 教练"映射与联动图。
- `README.md` 增加"建议的配合方式"与"反馈"。
- `release.yml` 增加 artifact 上传。

### 修正
- 论文诊断器删除"摘要 200–300 字"（高项**不写摘要**）。
- 备考路线改为"2024 年起**仅上半年**开考"。

## [0.2.0] - 2026-10-17

### 新增
- **11 个教练模块**（`coaches/`），统一六段式：R 原文锚点 / I 考生卡点 / A1 正确过程 / A2 反例库 / E 分层追问 / B 边界。
  - `01-itto-framework-coach` ITTO 框架教练
  - `02-mcq-diagnoser` 选择题诊断器
  - `03-evm-step-debugger` 挣值步骤纠错器
  - `04-cpm-reverse-checker` 关键路径逆向检查器
  - `05-case-finding-coach` 案例找茬教练
  - `06-essay-material-builder` 论文素材构建器
  - `07-essay-framework-diagnoser` 论文框架诊断器
  - `08-essay-anti-template` 论文反模板测试
  - `09-study-route-planner` 备考路线规划器
  - `10-daily-drill-scheduler` 每日微训练调度
  - `11-mistake-attribution-log` 错题归因日志
- `INDEX.md` 技能地图与触发速查。
- `examples/` 3 个"输入→输出"示例。
- `.github/workflows/release.yml`：打 tag 自动打包 zip。
- `LICENSE`（CC BY-NC-SA 4.0）。

### 变更
- `SKILL.md` 增加教练路由与"常见坑（Gotchas）"。
- `README.md` 重写：30 秒看懂、安装方式、教练清单、FAQ。

## [0.1.0] - 2026-10-16

### 新增
- 24 章知识框架（`chapters/`）。
- `SKILL.md` 主索引；`cheatsheet.md`、`glossary.md`、`patterns.md`。
- 初版 README 与版权声明。
