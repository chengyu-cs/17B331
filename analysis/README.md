# analysis/ — 风格分析层

文字存好了，还不够。她到底怎么说话的？主号一套、小号一套、演唱会上又一套。这层就是把这事量化了——句长、人称、隐喻、标点，全都算出来了。这层也没人做过！！

文件 | 内容
---|---
style_guide.md | 分语域文风指南：主号/小号/跨平台 caption/B站口语/演唱会 talking，五套语域怎么说话，全量化
style_stats_v3.md | 风格统计的口径和数字
style_labels.jsonl | 26,062 条逐条风格标注（年代/句长档/人称/隐喻域/修辞动作/emoji/感叹号），按 id 和主池关联
evidence_pool_curated.jsonl | 1,679 条精选证据，全部是她本人公开发言，带原始链接
exemplars.md | 场景样例：舞台开场、日常、演唱会这些场景的高置信片段，每条带 corpus id

两个注意：

- style_guide 的统计基于内部全量语料（44,641 条，比公开池大）。开头引用的文件名是内部文件。读的时候以这层的 style_stats_v3.md 为准～
- style_labels 约 80% 能直接 join 主池；剩下的指向没发布的早期内部版本，只有标签、没有文本。exemplars 每条的 corpus id 都能回 ../data/ 查原文。引用控制长度～
