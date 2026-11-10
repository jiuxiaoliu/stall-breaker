<div align="center">

# Stall Breaker

**把“我卡住了”变成可验证、可止损、可更新的下一步。**

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-111827?style=flat-square)](./SKILL.md)
[![Language](https://img.shields.io/badge/Language-中文-2563EB?style=flat-square)](./SKILL.md)
[![Status](https://img.shields.io/badge/Status-Active-16A34A?style=flat-square)](./SKILL.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-F59E0B?style=flat-square)](./LICENSE)

一个面向项目、研究、创作、经营、协作与高影响决策的停滞诊断 Skill。

</div>

---

## 它解决什么

很多“卡住”并不是执行力不足，而是问题问错、目标模糊、方向失效、信息缺失、资源受限或反馈断裂。`stall-breaker` 不急着给万能清单，而是先还原用户真正要完成的任务，再定位当前最限制结果的环节。

<p align="center">
  <code>表层请求</code> →
  <code>真实任务</code> →
  <code>主导瓶颈</code> →
  <code>竞争解释</code> →
  <code>跨期方案</code> →
  <code>当前最优</code> →
  <code>行动与复核</code>
</p>

它尤其适合这些表达：

- “项目推不动，但不知道卡在哪里。”
- “研究停滞了，继续读文献也没有进展。”
- “内容做不下去，感觉自己没有创意。”
- “方案很多，反而不知道选哪个。”
- “投入越来越多，结果始终没有改善。”
- “刚做了一个高风险决定，现在亏损很大。”

## 核心能力

| 能力 | 输出 |
| --- | --- |
| 真实需求识别 | 区分表层请求、待做决策、成功证据与反目标 |
| 停滞类型定位 | 从 12 类常见停滞中选择暂定主类型，并保留竞争解释 |
| 因果断点分析 | 从症状追到可改变变量，而不是平均优化所有环节 |
| 多时间尺度推演 | 同时检查眼前止损、近期验证、中期积累与长期锁定 |
| 方案比较与红队 | 淘汰不满足硬约束的路径，攻击排名第一的方案 |
| 可更新决策 | 给出当前最优解、止损线、翻转信号与复核节点 |

## 安装

### Codex

将仓库克隆到 Codex Skills 目录：

```bash
git clone https://github.com/jiuxiaoliu/stall-breaker.git ~/.codex/skills/stall-breaker
```

Windows PowerShell：

```powershell
git clone https://github.com/jiuxiaoliu/stall-breaker.git "$env:USERPROFILE\.codex\skills\stall-breaker"
```

重新打开 Codex 后，可以直接描述停滞场景；Skill 默认允许自动发现，也可以明确说“使用 stall-breaker 分析”。

## 使用示例

```text
我的研究停滞不前了。研究问题已经确定，但实验连续失败，
导师建议我继续增加样本。我不确定是方法错了还是数据不够。
```

```text
我做科普短视频，最好的一条 7000 播放，最差的只有 100 多。
我感觉自己没有创意了，帮我找真正的瓶颈和下一批验证选题。
```

```text
我前几天大量买入英伟达，现在跌了很多。
请先区分公司判断和我的资金结构风险，不要直接猜涨跌。
```

## 测试案例

仓库中的案例用于展示和回归测试，不是可直接复制的答案。

| 案例 | 主要测试点 |
| --- | --- |
| [科普短视频创作停滞](./cases/douyin-content-stall-2026-11-09.md) | 是否能从“没创意”转向受众承诺、选题机制、制作成本和反馈数据 |
| [英伟达集中持仓亏损](./cases/NVDA-leverage-2026-11-09.md) | 是否先处理杠杆、集中度和资金期限，而非预测短期股价 |
| [AI 广告视频服务获客](./cases/ai-video-sales-2026-11-09.md) | 是否识别联系人、信任证据与交易结构错配 |
| [家教平台停滞](./cases/tutoring-platform-round3-2026-11-09.md) | 是否根据实际产物修正用户自述和早期判断 |

## 目录

```text
stall-breaker/
├── SKILL.md
├── README.md
├── LICENSE
├── references/
│   ├── intent-and-scenario.md
│   ├── scoring-and-iteration.md
│   ├── service-productization.md
│   ├── stall-types.md
│   └── time-horizon.md
└── cases/
    ├── douyin-content-stall-2026-11-09.md
    ├── NVDA-leverage-2026-11-09.md
    └── ...
```

## 设计原则

- 类型是检索假设，不是给用户贴标签。
- 信息不足时可以假设推进，但必须降低结论强度。
- 不用固定三方案、固定 48 小时或固定评分制造形式完整。
- 下一步应产生决策信息，而不只是制造忙碌。
- 高风险问题先控制下行，再讨论收益。
- 历史案例不作为当前事实、行情或专业指令。

## 边界

本 Skill 不替代医疗、法律、财务等持牌专业服务。涉及重大财务、公共安全、解雇、离婚、合规或其他不可逆决策时，它只提供问题结构、风险控制与复核框架，并要求核验时效性事实。

## 参与改进

欢迎提交 Issue，最好包含：原始请求、Skill 的实际回答、哪里失焦、哪些新证据改变了判断。真实失败案例比抽象功能建议更有价值。

## 许可证

本项目采用 [MIT License](./LICENSE)。你可以自由使用、复制、修改、合并、发布和分发，但须保留原始版权声明与许可声明。

