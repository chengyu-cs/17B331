# data/ — 主池

她说过的话，全在这了！！三个文件，从公开平台一手洗出来的，一条条都带出处。每个字段什么意思看 ../docs/fields.md，怎么洗的看 ../docs/stats.md。

文件 | 内容 | 条数
---|---|---
corpus_public_safe_all.jsonl | 主池全量：bilibili 31,169 / weibo 2,408 / douyin 327 / wechat 260 / xhs 163 / concert 14 | 34,341
weibo_public_safe.jsonl | 微博子集。大号条目带 source_url 原微博链接；小号（alt 账号，804 条）链接在 provenance.url | 2,408
concert_talking.jsonl | 演唱会现场讲话（录音转写） | 14

用之前说三件事：

- 41 条 use_policy = generation_allowed_paraphrase_only（2018 艺考专访，粉丝剪辑、单来源）：引用请转述、别逐字长引。
- 微博小号条目 verified = false（single-source），用的时候自己交叉核实一下。
- 时间范围 2014-09-03 → 2026-10-22。按月翻、按视频翻，去 ../index/。
