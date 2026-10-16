# 高项公众号图文生产流（writing_flow）

本文件是 **`gaoxiang-di4ban-jiaocai`（高项第4版框架库）skill** 与**公众号写作/推送流**的衔接 SOP。
写高项（信息系统项目管理师）公众号图文时，按本 flow 走：从 skill 取框架层内容 → 套公众号合规模板 → 配图 → 自检 → 推草稿箱。

> 目标：产出**第4版合规**、**排版通过微信接口**、**可直接群发**的高项图文。
> 底层逐句原文在 `D:\WorkBuddy\Claw\01_备考资料\高项\高项教材知识库\`（24 章 markdown），本 skill 每条都标了章号，可回查。

---

## 0. 流程总览

```
① 选题定主题
   └─ 查 SKILL.md 的 Chapter Index / Topic Index 定位章号
② 取料（框架层）
   ├─ 读 chapters/chNN-*.md  → Core Idea / Frameworks / Key Concepts / Mental Models / Anti-patterns
   ├─ 公式·过程清单          → cheatsheet.md
   ├─ 术语·定义              → glossary.md
   ├─ 案例找错·论文技法·计算  → patterns.md
   └─ 需逐句原文             → D:\WorkBuddy\Claw\01_备考资料\高项\高项教材知识库\（按章号回查）
③ 套版（公众号 HTML 模板，见下方 §2）
④ 配图（官方截图红框 + 原创示意图，见 §3）
⑤ 合规自检（§4）
⑥ 推送草稿箱（§5）
```

---

## 1. 取料映射表（主题 → skill 文件）

| 文章主题 | 读哪个文件 | 配套取料 |
|---|---|---|
| 信息化/数字中国 | chapters/ch01-xinxi-fazhan.md | glossary（信息化6要素） |
| 新技术（云/AI/区块链） | chapters/ch02-xinxi-jishu.md | — |
| IT治理/IT审计 | chapters/ch03-xinxixitong-zhili.md | — |
| 12原则/价值驱动体系 | chapters/ch06-xiangmu-gailun.md | cheatsheet（12原则） |
| 立项/可行性研究 | chapters/ch07-xiangmu-lixiang.md | — |
| 整合/整体变更控制 | chapters/ch08-zhenghe.md | cheatsheet（变更流程） |
| 范围/WBS/确认范围 | chapters/ch09-fanwei.md | cheatsheet（WBS 要点） |
| 进度/关键路径/进度压缩 | chapters/ch10-jindu.md | cheatsheet（网络图·压缩） |
| 成本/挣值 EVM | chapters/ch11-chengben.md | cheatsheet（EVM 公式） |
| 质量/管理质量vs控制质量 | chapters/ch12-zhiliang.md | patterns（找错反模式） |
| 资源/估算活动资源 | chapters/ch13-ziyuan.md | — |
| 沟通/沟通模型 | chapters/ch14-goutong.md | — |
| 风险/定性与定量/应急 | chapters/ch15-fengxian.md | patterns（风险应对） |
| 采购/合同类型 | chapters/ch16-caigou.md | cheatsheet（合同类型） |
| 干系人/权力利益方格 | chapters/ch17-ganxishiren.md | — |
| **8个绩效域**（命题热点） | chapters/ch18-jixiaoyu.md | cheatsheet（绩效域清单） |
| 配置与变更 | chapters/ch19-peizhi-biangeng.md | — |
| 高级项目/量化管理 | chapters/ch20-gaoji.md | — |
| **计算（EMV/线性规划/博弈/指派）** | chapters/ch21-kexue-jichu.md | cheatsheet（计算套路） |
| 招投标/合同法/著作权 | chapters/ch24-falv-biaozhun.md | — |
| 案例找错 | patterns.md（反模式段） | cheatsheet（决策规则） |
| 论文写法 | patterns.md（论文技法段）+ cheatsheet（论文四段式） | — |

> 注意：高项**仅上半年（5月）开考**，下半年不开高项。文中涉及考试时点务必写明"高项仅上半年考"，避免误导下半年备考读者（下半年开考高级为系规/架构/分析师/网规）。

---

## 2. 公众号 HTML 模板（合规，直接复制改）

单 `<div>` 容器、内联样式、平铺语义标签（**不嵌套 div/section 盒子**）。

```html
<div style="max-width:680px;margin:0 auto;padding:18px 16px 40px;font-size:16px;line-height:1.8;color:#222;font-family:-apple-system,'PingFang SC','Microsoft YaHei',sans-serif;">
  <h1 style="font-size:22px;font-weight:bold;color:#1F3A5F;margin:0 0 16px;">文章标题</h1>

  <p style="margin:14px 0;">正文段落。必背词用 <span style="color:#d7263d;font-weight:bold;">红字</span>，理解词用 <span style="color:#1d6fb8;font-weight:bold;">蓝字</span>，口诀用 <span style="color:#2a9d4a;font-weight:bold;">绿字</span>。</p>

  <h2 style="font-size:18px;font-weight:bold;color:#222;border-bottom:2px solid #3b6cff;padding-bottom:6px;margin:24px 0 12px;">一、小节标题</h2>

  <p style="margin:14px 0;padding:10px 12px;border-left:3px solid #d7263d;background:#fdeef0;">提示框（callout）：用 border-left 色块，不用 box-shadow。</p>

  <table style="width:100%;border-collapse:collapse;margin:14px 0;font-size:15px;">
    <tr><th style="background:#1F3A5F;color:#fff;padding:8px 10px;border:1px solid #ccc;text-align:left;">列1</th><th style="background:#1F3A5F;color:#fff;padding:8px 10px;border:1px solid #ccc;text-align:left;">列2</th></tr>
    <tr><td style="padding:8px 10px;border:1px solid #ccc;">内容</td><td style="padding:8px 10px;border:1px solid #ccc;">内容</td></tr>
  </table>

  <p style="margin:14px 0;">图示：</p>
  <img src="fig_xxx.png" style="width:100%;display:block;border-radius:8px;margin:8px 0;">
  <p style="color:#999;font-size:13px;margin:4px 0 14px;">图注：说明这张图讲什么（截图需注明来源/示意图注明"非真实系统截图"）</p>

  <p style="margin:14px 0;color:#666;">结尾段。关于高项/中项/系规备考资料，后台回复关键词或看往期内容。</p>
</div>
```

**强制排版规则（微信接口过滤，必须守）：**
- 单容器：`max-width:680px;margin:0 auto;padding:18px 16px 40px;font-size:16px;line-height:1.8`
- 三色高亮用 `<span>`（**不用盒子**）：必背 `#d7263d` / 理解 `#1d6fb8` / 口诀 `#2a9d4a`
- 小标题 h2：18px + `border-bottom:2px solid #3b6cff`
- 色块 callout：用 `border-left:3px solid` + `padding:10px 12px` + 浅底，**禁用 box-shadow**
- 表头蓝底写在 `<th>` 级（微信丢弃 `<tr>` 上的 background）
- 有序列表：微信 `<ol><li>` 序号会翻倍 → 用 `list-style:none` 并手写"1. 2. 3."
- 图：`<img style="width:100%;display:block;border-radius:8px">`；图注 `#999;13px`
- 平铺语义标签，**不嵌套 div/section 盒子**；不用 `<style>` class 选择器
- **禁用样式**（自检 grep 应为 0）：`box-shadow` / `linear-gradient` / `letter-spacing` / `position` / `float` / `flex`

---

## 3. 配图

- **官方真实截图**（优先，更可信）：用 Playwright 截 `ruankao.org.cn` / `bm.ruankao.org.cn` 的公开页（首页、模拟练习入口、准考证打印按钮、通告页），红框标注关键信息。参考 `D:\WorkBuddy\Claw\02_公众号资料\公众号文章\gen_mock_shots.py` 的 `annotate()` 函数（红框坐标用 0–1 比例）。
- **需凭证/登录后界面**（截不到）：画**原创仿真示意图**，必须注明"非真实系统截图"，不盗用他人文章配图（版权意识）。
- **封面**：900×383，白底 + 顶部 150px 蓝块 `#3b6cff` + 主标题 46pt + 副标 22pt + 底条 `#f5f7fa` + "软考高项自习室·备考陪跑"。参考 `D:\WorkBuddy\Claw\02_公众号资料\公众号文章\gen_cover_examweek.py`。

---

## 4. 合规自检（发布前必跑）

1. **排版接口过滤**：`grep -E "box-shadow|linear-gradient|letter-spacing|position|float|flex" <file>.html` 应为 0 命中。
2. **第4版术语核对**（教材 0 命中的词一律不用）：
   - "八大绩效域" → 写"**8 个绩效域**"
   - "制订"（如"制订进度计划"）非"制定"
   - 进度管理仅 **6 过程**（估算活动资源归第13章资源管理）
   - "建设团队 / 监督风险 / 管理质量 / 互动沟通 / 应急计划+触发条件"（非旧版"人力资源计划/开展风险分析/实施质量保证/交互式沟通/权变措施"）
   - 论文**四段式**（2025起取消摘要），字数上限 **3500**
3. **考试时点**：高项仅上半年（5月）考，勿写"下半年高项"。

---

## 5. 推送草稿箱

> 关键坑：Bash 每条命令是独立会话，**SOCKS 隧道必须和推送放在同一条命令里**（否则推送时 1080 已消失，报 40164）。

```bash
cd "D:/WorkBuddy/Claw"
# 1) 起 SOCKS 隧道（腾讯云出口已加白，根治 40164）+ 2) 推送（同一条命令）
ssh -fN -D 1080 -o BatchMode=yes -o StrictHostKeyChecking=no root@rkgx.site 2>/dev/null; sleep 3; \
"C:/Users/BDTY-KF/.workbuddy/binaries/python/envs/default/Scripts/python.exe" \
  02_公众号资料/公众号文章/push_html_to_draft.py \
  02_公众号资料/公众号文章/<你的文章>.html \
  --title "标题（同名会幂等覆盖旧稿）" \
  --digest "摘要，约70字，含核心关键词" \
  --cover 02_公众号资料/公众号文章/<封面>.png
```

- 脚本自动搜索凭证（多路径兼容）：脚本同目录 / 脚本上级的 wechat-article-skills/ / 当前目录 / 02_公众号资料/wechat-article-skills/aws.env（从 Claw 根目录跑即可命中）。
- **必须带 `--cover`**，否则草稿报 `40007`（缺封面）。
- 同名标题**先删旧稿再建新稿**（幂等），改稿重推安全，不会重复。
- 本地相对路径的 `<img>` 自动上传微信永久素材（mmbiz 链接），不会裂图。
- 微信 API 返回已用 utf-8 解码，同名匹配稳定。

推送后：打开 `https://mp.weixin.qq.com` → 内容管理 → 草稿箱，核对排版与图片后群发。

---

## 6. 与 2027 高项推送规划衔接

高项自 2024 起仅上半年考，2027 高项 = **2027 年 5 月**（具体等软考办 2–3 月公告）。三阶段节奏（每篇都走本 flow 取料→套版→配图→推送）：

| 阶段 | 时间 | 节奏 | 内容重点 |
|---|---|---|---|
| 筑基精讲 | 系规考后 11月–1月 | 周 2 篇（周二综合/周五案例论文轮换） | 第4版 24 章 + 绩效域全覆盖，过 ITTO |
| 强化刷题 | 2–3 月 | 周 3 篇 | 真题/模拟、计算专题（EMV/线性规划/博弈/指派）、双拼融合案例、论文考察清单 |
| 冲刺模考 | 4月–考前 | 周 3–4 篇 | 必背口诀、时政速记（十五五/AI安全框架2.0/数安法个保法）、论文限时训练、全真模考 |

> 时政热点模块见综合知识一本通附录4（C.4），冲刺期直接调用。

---

## 7. 自动化重启（避免再断更）

- 先恢复 **"每周发文提醒与备稿"**（周一 9:00）——纯提醒，零产出压力，把"该发"拉回意识。
- 新建 **"2027 高项周更"**：`FREQ=WEEKLY;BYDAY=TU,FR;BYHOUR=8`（替代之前不可持续的日更）。
- 所有自动化 `cwds` **必须指向 Claw 工作区**，不能指向 WorkBuddy 安装目录（否则更新器拒绝更新）。
- 重型"章节考点系列""报名日报推送"等，等教材/时间到位再单独开。
