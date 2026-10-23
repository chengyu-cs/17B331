# index/ — 考古导航

想按视频翻？按月份翻？都在这。138 个月，128 个视频，我挨个数了～

文件 | 内容
---|---
by_video.json | B 站 128 个视频的段落索引：{BV 号: 段落数}，配合主池条目 ID 前缀（bili-<BV号>-<段号>）定位某视频全部字幕段
by_month.json | 按月条目数（138 个月，合计 34,341），看她哪阵子话多、哪阵子在憋大招

举个例子！！查完段落数，用 jq 'select(.id|startswith("bili-BV1C54y127u6"))' ../data/corpus_public_safe_all.jsonl，这个视频的字幕段就全出来了。
