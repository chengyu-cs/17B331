# index/ — 考古导航索引

| 文件 | 内容 |
|---|---|
| `by_video.json` | B 站 128 个视频的段落索引：`{BV 号: 段落数}`，配合主池条目 ID 前缀（`bili-<BV号>-<段号>`）定位某视频全部字幕段 |
| `by_month.json` | 按月条目数（138 个月，合计 34,341），适合看她的活跃时段分布 |

示例：查某视频段落数后，用 `jq 'select(.id|startswith("bili-BV1C54y127u6"))' ../data/corpus_public_safe_all.jsonl` 拉出该视频全部条目。
