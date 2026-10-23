# 字段说明

主池每个字段是什么，一条一条写清楚了。看不懂哪个，对着查～

- `id`：全局唯一 ID：weibo-{微博mid} / bili-{BV号}-{段序} / 其他平台同理
- `platform`：weibo / bilibili / douyin / wechat / xhs / concert
- `source_url`：原始公开链接（B站链接由 BV 号推导，标注于 README）
- `source_type`：采集通道类型
- `source_owner`：发言者归属（本池全部为 her）
- `date`：发布/上传日期（YYYY-MM-DD 或空）
- `title`：视频/微博标题
- `text`：正文文本（字幕段/微博正文/现场讲话）
- `verified` / `verification`：来源核验标记
- `language` / `tags` / `metrics` / `images` / `has_video`：元信息
- `sensitive_period`：敏感期标记（已过滤，本池仅保留公开安全条目）
- `speaker` / `speaker_confidence`：B站字幕说话人归属及置信度（入池阈值 ≥0.72；另有 5 个视频共 46 条 0.65 段如实保留，见 stats.md）
- `is_compilation` / `source_layer` / `channel`：分层与合集标记
- `use_policy`：使用策略：public_safe_generation（公开安全生成）/ generation_allowed_paraphrase_only（仅限转述，41 条 2018 艺考剪辑）
- `checksum`：文本校验和

就这些！！对不上的时候，回主池查原文，别猜～
