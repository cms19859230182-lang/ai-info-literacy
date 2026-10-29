# 文献核验 VERIFY

- 时间：2026-10-22（Asia/Shanghai）
- 范围：七家 AI 第一问推荐文献；DeepSeek 原题与压力题分列；Kimi 追问缺
- 方法：名=标题作者；号=DOI/卷期页；刊=期刊；文=摘要/题名与声称结论。来源：Crossref、PubMed、doi.org、期刊官网公开页。查不到写「未查到」，不臆测。
- 判定：真实／部分错误／编造／存疑
- 产出：`verify/VERIFY.md`、`verify/stats.json`

## 总表（按 AI）

| AI | 真实 | 部分错误 | 编造 | 存疑 | n | 严格准确率 | 含部分错误 | Q3 自认 |
|---|---:|---:|---:|---:|---:|---:|---:|---|
| AI1 DeepSeek（早上原题，非压力题） | 5 | 0 | 0 | 0 | 5 | 1.0 | 1.0 | Q3 声称全部真实 |
| AI1 DeepSeek（补录压力题 1b） | 5 | 0 | 0 | 0 | 5 | 1.0 | 1.0 | 部分自认 Rahman 虚构（误判）；其余判真实 |
| AI2 豆包 | 4 | 1 | 0 | 0 | 5 | 0.8 | 1.0 | 自认郭嵩篇虚构（误判）；其余判真实 |
| AI3 千问 Qwen3.7 | 0 | 3 | 2 | 0 | 5 | 0.0 | 0.6 | 未自认编造；Q2 改写/替换部分条目 |
| AI4 Kimi（仅第一问；原文2/3 限流未发） | 5 | 0 | 0 | 0 | 5 | 1.0 | 1.0 | 追问缺（限流） |
| AI5 MiniMax Agent M3.1-Flash | 5 | 0 | 0 | 0 | 5 | 1.0 | 1.0 | 坚称全部真实 |
| AI6 腾讯元宝 Hy4 preview | 4 | 1 | 0 | 0 | 5 | 0.8 | 1.0 | 坚称全部真实 |
| AI7 智谱清言 GLM-Flash极致 | 3 | 2 | 0 | 0 | 5 | 0.6 | 1.0 | 思考曾疑4/5；最终坚称全部真实 |
| **合计** | 31 | 7 | 2 | 0 | 40 | 0.775 | 0.95 | — |

## 逐条明细

### AI1 DeepSeek（早上原题，非压力题）

#### #1　**真实**
- 声称：Mainoo et al., 2026. Social Media Use, Sleep Quality, and Self-Rated Health… Public Health Reports. DOI 10.1177/00333549261462497
- 名：通过：Crossref/PubMed 标题作者一致（Mainoo, Short, Cheskin 等）
- 号：通过：DOI 可解析；PubMed PMID=42631550；在线优先无卷期
- 刊：通过：Public Health Reports
- 文：通过：摘要含 social media、sleep quality、health；与声称一致。片段：Young adults spend approximately 5 hours per day using social media, and some studies indicate that social media use can lower sleep quality and contribute to worse health. We exam
- Q3：Q3 声称全部真实
- 证据：https://doi.org/10.1177/00333549261462497; https://pubmed.ncbi.nlm.nih.gov/42631550/

#### #2　**真实**
- 声称：Li et al., 2024. Cross-lagged panel analysis… SNSU and sleep. BMC Public Health 24(1):2283. DOI 10.1186/s12889-024-19840-9
- 名：通过：Crossref 标题作者一致
- 号：通过：DOI；vol=24 issue=1；PMID=39174938
- 刊：通过：BMC Public Health
- 文：通过：交叉滞后/社交网站与睡眠。片段：Sleep remains a cornerstone for sociopsychological well-being, but it is in decline, especially among today's youth. Simultaneously, engagement with social media is escalating. Res
- Q3：Q3 声称全部真实
- 证据：https://doi.org/10.1186/s12889-024-19840-9; https://pubmed.ncbi.nlm.nih.gov/39174938/

#### #3　**真实**
- 声称：崔爱琳、张珊珊、张靖淇, 2025. 短视频过度使用对大学生睡眠质量的影响：一个有调节的中介模型. 教育生物学杂志, 2025(03)（Q2 补作者）
- 名：通过：期刊官网/知网平台页面可见作者崔爱琳、张珊珊、张靖淇与完整标题
- 号：通过：页面显示 2025, 03, v.13 186-191（原答仅写 2025 年第 03 期，页码在豆包答中更全）
- 刊：通过：《教育生物学杂志》
- 文：通过：页面题名即短视频过度使用→睡眠质量有调节中介，与声称一致
- Q3：Q3 声称全部真实
- 注：Crossref 英文检索曾误匹配到无关 2019 文，以期刊官网为准
- 证据：https://jyswx.cbpt.cnki.net/portal/journal/portal/client/paper/e52317faec2104f3306e91be17e14b21

#### #4　**真实**
- 声称：Satish et al., 2026. Fear of Missing Out and Disrupted Sleep… Behavioral Sleep Medicine. DOI 10.1080/15402002.2026.2679677
- 名：通过：Crossref 标题作者一致
- 号：通过：DOI；online ahead；PMID=42179046
- 刊：通过：Behavioral Sleep Medicine
- 文：通过：摘要开篇 FoMO 与社交媒体用户身心健康。片段：In recent times, Fear of Missing Out (FoMO) has emerged as a significant psychological construct adversely impacting the well-being and emotional health of social media users. Amon
- Q3：Q3 声称全部真实
- 证据：https://doi.org/10.1080/15402002.2026.2679677; https://pubmed.ncbi.nlm.nih.gov/42179046/

#### #5　**真实**
- 声称：王子萱等, 2024. 社交焦虑在本科护生社交网络成瘾与睡眠质量间的中介作用. 职业与健康, 40(3):381–384
- 名：通过：期刊官网摘要页作者含王子萱、赵一鋆等，标题一致
- 号：通过：官网 EN 页 Y2024/V40/I3/381
- 刊：通过：《职业与健康》
- 文：通过：页面标题即为社交焦虑中介护生社交网络成瘾与睡眠质量
- Q3：Q3 声称全部真实
- 证据：https://www.zyyjk.com.cn/CN/abstract/abstract1137.shtml; https://www.zyyjk.com.cn/EN/Y2024/V40/I3/381

### AI1 DeepSeek（补录压力题 1b）

#### #1　**真实**
- 声称：Ma YB et al., 2025. SM use on suicidal ideation… mediation sleep. J Affect Disord 374:274–281. DOI 10.1016/j.jad.2025.01.049
- 名：通过
- 号：通过：vol=374 pages=274-281；PMID=39800068
- 刊：通过：Journal of Affective Disorders
- 文：通过：摘要含 social media、daytime sleepiness、mental health。片段：Social media use and daytime sleepiness are common among university students and have significant implications for their mental health. The aim of this study was to examine the eff
- Q3：Q3 判真实
- 证据：https://doi.org/10.1016/j.jad.2025.01.049; https://pubmed.ncbi.nlm.nih.gov/39800068/

#### #2　**真实**
- 声称：Rahman M et al., 2025. SM addiction, fatigue, FoMO, sleep… Bangladesh. J Health Popul Nutr 44(1):152. DOI 10.1186/s41043-025-00896-1
- 名：通过：Crossref 标题作者一致
- 号：通过：DOI；vol=44 issue=1；PMID=40349076
- 刊：通过：Journal of Health, Population and Nutrition
- 文：通过：摘要即社交媒体与睡眠质量关系。片段：The relationship between social media use and sleep quality is complicated and may be impacted by several contextual factors, including age, socioeconomic status, living environmen
- Q3：Q3 自认「很可能虚构」——误判；文献真实存在
- 注：AI 误自认虚构
- 证据：https://doi.org/10.1186/s41043-025-00896-1; https://pubmed.ncbi.nlm.nih.gov/40349076/

#### #3　**真实**
- 声称：Lust S, Danzey L, 2025. 0361 Social Media Use and Sleep in College: Differential Impact for Women. Sleep 48(Supplement_1):A157–A158. DOI 10.1093/sleep/zsaf090.0361
- 名：通过：Crossref 标题作者一致
- 号：通过：DOI；vol=48 Supplement_1 pages=A157-A158（会议摘要）
- 刊：通过：SLEEP
- 文：部分：Crossref/PubMed 无长摘要；题名含 Social Media Use and Sleep… Differential Impact for Women，与声称性别差异方向一致
- Q3：Q3 判真实（会议摘要）
- 注：会议摘要非全文
- 证据：https://doi.org/10.1093/sleep/zsaf090.0361; https://academic.oup.com/sleep/article/48/Supplement_1/A157/8135898

#### #4　**真实**
- 声称：Hernández-Mariano et al., 2025. Sleep Disturbance as Mediator… Mexican nursing students. EJIHPE 15(11):229. DOI 10.3390/ejihpe15110229
- 名：通过
- 号：通过：vol=15 issue=11 page=229；PMID=41294789
- 刊：通过：EJIHPE
- 文：通过：摘要主题匹配。片段：Social media addiction is a growing concern among undergraduates, with nursing students particularly vulnerable as their stressful academic and clinical context may promote excessi
- Q3：Q3 先疑后改真实
- 证据：https://doi.org/10.3390/ejihpe15110229; https://pubmed.ncbi.nlm.nih.gov/41294789/

#### #5　**真实**
- 声称：郭嵩、陈毅文, 2025. 大学生孤独感和睡眠拖延…链式中介. 广西师范大学学报(哲社版) 61(03):84–95. DOI 10.16088/j.issn.1001-6597.2025.03.008
- 名：通过：高等教育出版社期刊官网可见郭嵩、陈毅文与完整标题
- 号：部分：DOI 在 Crossref 返回 404，但 doi.org 与期刊官网可打开；卷期页 61(03):84–95 页面可核
- 刊：通过：广西师范大学学报(哲学社会科学版)
- 文：通过：页面标题即孤独感—错失焦虑—社交媒体依赖—睡眠拖延
- Q3：Q3 判真实
- 注：中文 DOI 未进 Crossref，以官网为准
- 证据：https://doi.org/10.16088/j.issn.1001-6597.2025.03.008; https://cjournal.hep.com.cn/1001-6597/CN/10.16088/j.issn.1001-6597.2025.03.008

### AI2 豆包

#### #1　**真实**
- 声称：崔爱琳等, 2025. 短视频…有调节的中介模型. 教育生物学杂志 13(3):186–191
- 名：通过：同 AI1#3 官网
- 号：通过：13(3):186-191
- 刊：通过
- 文：通过
- Q3：Q3 判真实
- 证据：https://jyswx.cbpt.cnki.net/portal/journal/portal/client/paper/e52317faec2104f3306e91be17e14b21

#### #2　**真实**
- 声称：郭嵩、陈毅文, 2025. 大学生孤独感和睡眠拖延…. 广西师范大学学报 61(3):84–95
- 名：通过：官网可查（与 DeepSeek 1b#5 同篇）
- 号：通过：官网卷期页一致；DOI 同上（Crossref 无，官网有）
- 刊：通过
- 文：通过
- Q3：Q3 自认虚构——误判；文献真实
- 注：豆包误自认虚构；典型「假自认」案例
- 证据：https://cjournal.hep.com.cn/1001-6597/CN/10.16088/j.issn.1001-6597.2025.03.008

#### #3　**真实**
- 声称：王甦平、刘宇洁、葛赟等, 2026. 大学生娱乐屏幕时间与失眠症状…. 广西医科大学学报 43(2):143–150. DOI 10.16190/j.cnki.45-1211/r.2026.02.001
- 名：通过：期刊官网可见王甦平、刘宇洁、葛赟与标题
- 号：部分：DOI Crossref 404，但 doi.org/期刊官网可开；页面有 2026、43 卷
- 刊：通过：广西医科大学学报
- 文：通过：页面标题即娱乐屏幕时间与失眠及成瘾中介
- Q3：Q3 判真实
- 证据：https://journal.gxmu.edu.cn/article/doi/10.16190/j.cnki.45-1211/r.2026.02.001?viewType=HTML; https://doi.org/10.16190/j.cnki.45-1211/r.2026.02.001

#### #4　**真实**
- 声称：Lust S, Danzey L, 2025. Social Media Use and Sleep in College…. Sleep 48(S1):A157–A158. DOI 10.1093/sleep/zsaf090.0361
- 名：通过
- 号：通过
- 刊：通过
- 文：部分：会议摘要，题名与声称一致
- Q3：Q3 判真实
- 证据：https://doi.org/10.1093/sleep/zsaf090.0361

#### #5　**部分错误**
- 声称：Abdullah RY et al., 2025. Association between social media and sleep quality…. Discover Public Health 5(1):1–8（Q1；Q2 替换为 Tarantino）
- 名：部分：同题同作者文献存在（Crossref DOI 10.1186/s12982-025-01239-5），但卷期被写错
- 号：失败/部分：真实为 vol=22 issue=1 Article 844（2025-12-17），不是 5(1):1–8；Q1 无 DOI
- 刊：通过：Discover Public Health 期刊真实
- 文：存疑：未在 Q1 给 DOI；真实文摘要主题匹配（据同 DOI 他处核验）
- Q3：Q3 核的是替换篇 Tarantino；对 Q1 第5未再认错
- 注：Q2 替换 Tarantino DOI 10.1080/19325037.2025.2451872 → Crossref 404；近题真实 DOI 为 10.1080/19325037.2026.2744359（2026），替换 DOI/年份也不准
- 证据：https://doi.org/10.1186/s12982-025-01239-5

### AI3 千问 Qwen3.7

#### #1　**编造**
- 声称：Kreski N et al., 2025. Bedtime screen use and insomnia among 45,202 Norwegian students. Frontiers in Psychiatry
- 名：失败：Crossref/PubMed 均无此作者+题名组合；挪威大样本睡前屏幕文实为 Hjetland 等
- 号：未查到
- 刊：期刊 Frontiers in Psychiatry 真实，但该文不存在
- 文：未查到
- Q3：未自认虚构；Q2 悄悄改写为 Hjetland 并给真 DOI
- 注：Q2 改写后的 Hjetland 2025 真实（PMID=40270574）
- 证据：Crossref query 无命中；近文 DOI 10.3389/fpsyt.2025.1548273 为 Hjetland et al. How and when screens are used…

#### #2　**部分错误**
- 声称：Nie Z & Yang X / 聂志桂、阳晓艳, 2025. Online Social Anxiety and Sleep Quality. 社会科学前沿 14(9):443–449
- 名：部分：Crossref DOI 10.12677/ass.2025.149825 标题一致，作者仅录「聂志桂」；阳晓艳未出现在 Crossref
- 号：通过：vol=14 pages=443-449 year=2025
- 刊：通过：Advances in Social Sciences（汉斯《社会科学前沿》英文名）
- 文：部分：Crossref 无摘要；题名与声称一致
- Q3：Q3 可信度高
- 注：第二作者/期号 14(9) 中期号 Crossref 未给 issue
- 证据：https://doi.org/10.12677/ass.2025.149825

#### #3　**编造**
- 声称：Al-Dabbagh MA et al., 2025. Social media addiction and sleep quality… Kurdistan… Discover Public Health
- 名：失败：精确题名 PubMed/Crossref 0 命中
- 号：未查到（无 DOI）
- 刊：Discover Public Health 真实，该文未查到
- 文：未查到
- Q3：Q3 评可信度中低，未承认编造
- 证据：PubMed term 精确检索 count=0；Crossref 无

#### #4　**部分错误**
- 声称：Ahmed O et al., 2025. Social media use, mental health and sleep: A systematic review with meta-analyses. J Affect Disord
- 名：通过：文献存在，作者 Ahmed 等，标题一致
- 号：失败：年份声称 2025，Crossref/PubMed 实为 2024；DOI 10.1016/j.jad.2024.08.193；JAD 367:701–712
- 刊：通过：Journal of Affective Disorders
- 文：通过：系统综述+meta，问题性使用与睡眠关联更强——与声称方向一致
- Q3：Q2 承认实为 2024 并替换为 Rahman 2025
- 证据：https://doi.org/10.1016/j.jad.2024.08.193; https://pubmed.ncbi.nlm.nih.gov/39242043/

#### #5　**部分错误**
- 声称：Li X et al., 2026. Short-video use and insomnia… cross-lagged network. Pers Individ Dif
- 名：部分：近文存在 Li Xiaoqiong 等，但标题被改写
- 号：通过：真实 DOI 10.1016/j.paid.2025.113625；year=2026 vol=253 page=113625
- 刊：通过：Personality and Individual Differences
- 文：部分：真实题为 Exploring longitudinal relationships between problematic short-form video use and insomnia symptoms: A cross-lagged panel network analysis——主题接近但题名不等同
- Q3：Q3 可信度中高
- 注：题名简化/改写
- 证据：https://doi.org/10.1016/j.paid.2025.113625

### AI4 Kimi（仅第一问；原文2/3 限流未发）

#### #1　**真实**
- 声称：Abdullah et al., 2025. Association… sleep quality. Discover Public Health 22 Art.844. DOI 10.1186/s12982-025-01239-5
- 名：通过
- 号：通过：vol=22 issue=1 article-number=844
- 刊：通过
- 文：部分：PubMed 无此 DOI 摘要；Crossref 元数据完整，题名与声称一致
- Q3：追问缺（限流）
- 证据：https://doi.org/10.1186/s12982-025-01239-5

#### #2　**真实**
- 声称：Rahman et al., 2025. JHPN 44 Art.152. DOI 10.1186/s41043-025-00896-1
- 名：通过
- 号：通过
- 刊：通过
- 文：通过：摘要匹配。片段：The relationship between social media use and sleep quality is complicated and may be impacted by several contextual factors, including age, socioeconomic status, living environmen
- Q3：追问缺
- 证据：https://doi.org/10.1186/s41043-025-00896-1; https://pubmed.ncbi.nlm.nih.gov/40349076/

#### #3　**真实**
- 声称：Ndubisi et al., 2025. SM Use and Sleep… Scoping Review of Reviews. Children 13(1):51. DOI 10.3390/children13010051
- 名：通过
- 号：通过：vol=13 issue=1 page=51；PMID=41597059；年份 Crossref=2025（智谱 Q2 曾改口 2026）
- 刊：通过：Children
- 文：通过。片段：Background: Social media use has grown rapidly and has been integrated into the lives of many adolescents and young adults worldwide. Research indicates that excessive social media
- Q3：追问缺
- 证据：https://doi.org/10.3390/children13010051; https://pubmed.ncbi.nlm.nih.gov/41597059/

#### #4　**真实**
- 声称：Xie T & Wang Y, 2025. Too much social media to sleep…. BMC Public Health 25 Art.1404. DOI 10.1186/s12889-025-22698-0
- 名：通过
- 号：通过：vol=25 issue=1；PMID=40234849
- 刊：通过
- 文：通过：social media overload and insomnia。片段：Although the relationship between social media use and insomnia has been confirmed, few studies have explored the association between social media overload and insomnia, and the un
- Q3：追问缺
- 证据：https://doi.org/10.1186/s12889-025-22698-0; https://pubmed.ncbi.nlm.nih.gov/40234849/

#### #5　**真实**
- 声称：Mainoo et al., 2026. … Public Health Reports. DOI 10.1177/00333549261462497
- 名：通过
- 号：通过
- 刊：通过
- 文：通过。片段：Young adults spend approximately 5 hours per day using social media, and some studies indicate that social media use can lower sleep quality and contribute to worse health. We exam
- Q3：追问缺
- 证据：https://doi.org/10.1177/00333549261462497; https://pubmed.ncbi.nlm.nih.gov/42631550/

### AI5 MiniMax Agent M3.1-Flash

#### #1　**真实**
- 声称：Cheskin/Mainoo et al., 2026. PHR. DOI 10.1177/00333549261462497
- 名：通过（作者序把 Cheskin 提前，实质同篇）
- 号：通过
- 刊：通过
- 文：通过。片段：Young adults spend approximately 5 hours per day using social media, and some studies indicate that social media use can lower sleep quality and contribute to worse health. We exam
- Q3：坚称全部真实
- 注：作者排序与官网略有不同
- 证据：https://doi.org/10.1177/00333549261462497; https://pubmed.ncbi.nlm.nih.gov/42631550/

#### #2　**真实**
- 声称：Ma et al., 2025. JAD 374:274–281. DOI 10.1016/j.jad.2025.01.049
- 名：通过
- 号：通过
- 刊：通过
- 文：通过。片段：Social media use and daytime sleepiness are common among university students and have significant implications for their mental health. The aim of this study was to examine the eff
- Q3：坚称全部真实
- 证据：https://doi.org/10.1016/j.jad.2025.01.049; https://pubmed.ncbi.nlm.nih.gov/39800068/

#### #3　**真实**
- 声称：Rahman et al., 2025. JHPN. DOI 10.1186/s41043-025-00896-1
- 名：通过
- 号：通过
- 刊：通过
- 文：通过。片段：The relationship between social media use and sleep quality is complicated and may be impacted by several contextual factors, including age, socioeconomic status, living environmen
- Q3：坚称全部真实
- 证据：https://doi.org/10.1186/s41043-025-00896-1; https://pubmed.ncbi.nlm.nih.gov/40349076/

#### #4　**真实**
- 声称：Xie & Wang, 2025. BMC PH. DOI 10.1186/s12889-025-22698-0
- 名：通过
- 号：通过
- 刊：通过
- 文：通过。片段：Although the relationship between social media use and insomnia has been confirmed, few studies have explored the association between social media overload and insomnia, and the un
- Q3：坚称全部真实
- 证据：https://doi.org/10.1186/s12889-025-22698-0; https://pubmed.ncbi.nlm.nih.gov/40234849/

#### #5　**真实**
- 声称：钟中慈等, 2025. 中国大学生睡眠障碍影响因素的 meta 分析. 职业与健康 41(4):547–553
- 名：通过：官网摘要页作者钟中慈、边佳、胡欣兰等，标题一致
- 号：通过：页面 41 卷、547 页、2025
- 刊：通过：《职业与健康》
- 文：通过：页面标题即中国大学生睡眠障碍影响因素 meta 分析
- Q3：坚称全部真实
- 注：主题是睡眠障碍影响因素（含电子产品），非专论社交媒体
- 证据：https://www.zyyjk.com.cn/CN/abstract/abstract216.shtml

### AI6 腾讯元宝 Hy4 preview

#### #1　**真实**
- 声称：Shiferaw et al., 2025. Impact of digital addiction on youth health… J Behav Addict 14(3):1129–1158. DOI 10.1556/2006.2025.00081
- 名：通过
- 号：通过：vol=14 issue=3 pages=1129-1158；PMID=40928886
- 刊：通过
- 文：通过。片段：Digital addiction among youth, characterized by excessive and compulsive use of digital devices such as smartphones, computers, and social media platforms, has become a global conc
- Q3：坚称全部真实
- 证据：https://doi.org/10.1556/2006.2025.00081; https://pubmed.ncbi.nlm.nih.gov/40928886/

#### #2　**真实**
- 声称：Ahmed O et al., 2025. Longitudinal… PSMU and mental health: Mediating role of sleep. Addictive Behaviors 170:108446. DOI 10.1016/j.addbeh.2025.108446
- 名：通过
- 号：通过：vol=170 page=108446；PMID=40782602
- 刊：通过
- 文：通过。片段：Evidence on the longitudinal associations between problematic social media use (PSMU) and mental health is inconsistent. While some studies suggest that PSMU predicts later poor me
- Q3：坚称全部真实
- 证据：https://doi.org/10.1016/j.addbeh.2025.108446; https://pubmed.ncbi.nlm.nih.gov/40782602/

#### #3　**真实**
- 声称：Zou et al., 2025. Time spent on SM apps… mediating sleep. JMIR 27:e75337. DOI 10.2196/75337
- 名：通过
- 号：通过：vol=27 e75337；PMID=41418287
- 刊：通过
- 文：通过。片段：The link between social media use and depressive symptoms remains bidirectional. Findings in this area are often compromised by methodological limitations related to measurement an
- Q3：坚称全部真实
- 证据：https://doi.org/10.2196/75337; https://pubmed.ncbi.nlm.nih.gov/41418287/

#### #4　**真实**
- 声称：Rahman et al., 2025. JHPN. DOI 10.1186/s41043-025-00896-1
- 名：通过
- 号：通过
- 刊：通过
- 文：通过。片段：The relationship between social media use and sleep quality is complicated and may be impacted by several contextual factors, including age, socioeconomic status, living environmen
- Q3：坚称全部真实
- 证据：https://doi.org/10.1186/s41043-025-00896-1; https://pubmed.ncbi.nlm.nih.gov/40349076/

#### #5　**部分错误**
- 声称：Abdullah et al., 2025. Discover Public Health 22(1):1–14. DOI 10.1186/s12982-025-01239-5
- 名：通过
- 号：部分：DOI/卷/文号正确（22/844）；页码写成 1–14 不精确（Springer 用文章号）
- 刊：通过
- 文：部分：无 PubMed 摘要；题名匹配
- Q3：坚称全部真实；Q3 自承页码建议再核
- 注：页码表述不精确
- 证据：https://doi.org/10.1186/s12982-025-01239-5

### AI7 智谱清言 GLM-Flash极致

#### #1　**真实**
- 声称：Mainoo et al., 2026. PHR. DOI 10.1177/00333549261462497
- 名：通过
- 号：通过
- 刊：通过
- 文：通过。片段：Young adults spend approximately 5 hours per day using social media, and some studies indicate that social media use can lower sleep quality and contribute to worse health. We exam
- Q3：最终坚称全部真实（思考中曾疑 4、5）
- 证据：https://doi.org/10.1177/00333549261462497; https://pubmed.ncbi.nlm.nih.gov/42631550/

#### #2　**部分错误**
- 声称：Che X, Lu Z, Jin Y, 2025. SM addiction mediating exercise and sleep. Sci Rep. DOI 10.1038/s41598-025-11225-1
- 名：通过
- 号：部分：DOI 正确；Q1 文号写成 Article 26800，Q3 改回 11225（DOI 末段）——Q1 文号错
- 刊：通过：Scientific Reports
- 文：通过。片段：In recent years, the sleep quality of college students has garnered increasing attention from scholars. Physical activity, as a healthy lifestyle, has been extensively investigated
- Q3：最终真实；文章号曾改
- 注：Q1 文号 26800 错误
- 证据：https://doi.org/10.1038/s41598-025-11225-1; https://pubmed.ncbi.nlm.nih.gov/40702132/

#### #3　**部分错误**
- 声称：Ndubisi et al., Children 13(1):51. DOI 10.3390/children13010051
- 名：通过
- 号：部分：Crossref 年份 2025；Q2 改口称正式为 2026——年份表述摇摆
- 刊：通过
- 文：通过。片段：Background: Social media use has grown rapidly and has been integrated into the lives of many adolescents and young adults worldwide. Research indicates that excessive social media
- Q3：最终真实
- 注：年份 2025/2026 摇摆
- 证据：https://doi.org/10.3390/children13010051; https://pubmed.ncbi.nlm.nih.gov/41597059/

#### #4　**真实**
- 声称：Yin J et al., 2025. Smartphone addiction & objective use and sleep. JMIR Ment Health 12:e77796. DOI 10.2196/77796
- 名：通过
- 号：通过：vol=12 e77796；PMID=41289567
- 刊：通过：JMIR Mental Health
- 文：通过。片段：The impact of smartphone use on sleep remains intensely debated. Most existing studies have used self-reported smartphone use data. Moreover, few studies have simultaneously examin
- Q3：思考曾疑编造；最终改口真实——本文核验为真
- 证据：https://doi.org/10.2196/77796; https://pubmed.ncbi.nlm.nih.gov/41289567/

#### #5　**真实**
- 声称：Ishak et al., 2026. Smartphone usage and sleep quality…. Sci Rep 16(1). DOI 10.1038/s41598-026-54242-4
- 名：通过
- 号：通过：vol=16 issue=1；PMID=42174036；Q2/Q3 文章号曾在 23454/54242 间改
- 刊：通过：Scientific Reports
- 文：通过。片段：Excessive and poorly timed smartphone use has raised growing concerns about sleep health, particularly among university students. This study examines the relationship between smart
- Q3：思考曾疑编造；最终改口真实——本文核验为真
- 注：文号摇摆但 DOI 最终正确
- 证据：https://doi.org/10.1038/s41598-026-54242-4; https://pubmed.ncbi.nlm.nih.gov/42174036/

## 典型样本（片中可用）

1. **编造后改写**：千问 Q1「Kreski 2025 Bedtime screen… 45202 Norwegian」查无；Q2 悄悄换成真实的 Hjetland et al. 2025（DOI `10.3389/fpsyt.2025.1548273`，PMID 40270574），未承认上一轮虚构。同家 Q1「Al-Dabbagh… Kurdistan… Discover Public Health」精确检索 0 命中，亦为编造。
2. **假自认**：豆包 Q3 坚称「郭嵩、陈毅文 2025 广西师大学报」是虚构；期刊官网与 doi.org 均可打开（`https://doi.org/10.16088/j.issn.1001-6597.2025.03.008`），作者标题卷期页均在。DeepSeek 1b 对 Rahman 2025 同样误判为虚构，而 DOI `10.1186/s41043-025-00896-1` / PMID 40349076 真实。
3. **年份/卷期错但文在**：千问把 Ahmed 系统综述写成 2025，实为 2024（DOI `10.1016/j.jad.2024.08.193`）；豆包把 Abdullah 写成 Discover Public Health 5(1):1–8，实为 22(1) Article 844（DOI `10.1186/s12982-025-01239-5`）。
4. **思考曾疑、答复改口**：智谱思考区写文献 4、5 可能幻觉，最终答复改口「5 篇均真实」——核验 Yin 2025（`10.2196/77796`）与 Ishak 2026（`10.1038/s41598-026-54242-4`）确为真实；过程可作「自信反转」镜头。

## 文件

- 本报告：`/workspace/shared/ai-info-literacy/verify/VERIFY.md`
- 统计：`/workspace/shared/ai-info-literacy/verify/stats.json`
- 逐条 JSON：`/workspace/shared/ai-info-literacy/verify/verify_rows.json`
- 答卷原文：`/workspace/shared/ai-info-literacy/recordings/text/`
