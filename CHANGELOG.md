# 更新日志

遵循 [语义化版本](https://semver.org/lang/zh-CN/)。

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
