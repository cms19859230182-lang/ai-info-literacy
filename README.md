# AI 信息素养 · 文献核验开源包（脱敏）

用公开文献库核验 AI 给出的参考文献，区分「全对／有错／查无此文」。本仓只放方法摘要、核验口径与脱敏答卷样例，**不含**登录态、Cookie、手机号、校园账号或浏览器 profile。

## 主口径（片内与本仓一致）

- **N = 603 = 79 全对 ／ 116 有错 ／ 408 查无此文**
- **六家工具**：DeepSeek、豆包、通义千问、MiniMax、腾讯混元、智谱清言
- **不含 Kimi**（不做七家口径）
- 公开样例正文按 **≥ 400 字** 收录

## 目录

| 路径 | 说明 |
|------|------|
| [`docs/METHOD.md`](docs/METHOD.md) | 方法说明（脱敏开源） |
| [`docs/VERIFY.md`](docs/VERIFY.md) | 文献核验口径与总表 |
| [`stats/stats.json`](stats/stats.json) | 按工具汇总的结构化统计 |
| [`samples/doubao/`](samples/doubao/) | 豆包脱敏答卷样例（3 份） |
| [`samples/yuanbao/`](samples/yuanbao/) | 腾讯元宝／混元脱敏答卷样例（3 份） |

## 怎么读

1. 先看 `docs/METHOD.md` 了解题干与判定口径。
2. 再看 `docs/VERIFY.md` 与 `stats/stats.json` 对照各工具表现。
3. `samples/` 下为脱敏正文，便于复现「如何核验」的阅读体验；**不是**完整原始对话导出。

## 隐私声明

本仓库刻意剥离：

- Cookie、会话 token、API key
- 手机号、邮箱、真实姓名与校园账号
- 本机路径与浏览器 profile

若你 fork 后自行补录原始答卷，请先脱敏再提交。

## 许可与用途

教学演示与方法复现。核验判定由人工完成；AI 仅用于生成被测文献条目、列检索词与整理表格。
