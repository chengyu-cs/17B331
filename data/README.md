# data/ — 清洗层主池

全部为黄霄雲本人的公开发言文本，入池前经"她本人段 + 说话人置信度 + 公开安全过滤"清洗（漏斗与例外披露见 ../docs/stats.md）。全字段说明见 ../docs/fields.md。

| 文件 | 内容 | 条数 |
|---|---|---|
| `corpus_public_safe_all.jsonl` | 主池全量：bilibili 31,169 / weibo 2,408 / douyin 327 / wechat 260 / xhs 163 / concert 14 | 34,341 |
| `weibo_public_safe.jsonl` | 微博子集。大号条目带 `source_url` 原微博链接；小号（alt 账号，804 条）链接在 `provenance.url` | 2,408 |
| `concert_talking.jsonl` | 演唱会现场讲话（录音转写） | 14 |

使用注意：

- 41 条 `use_policy = generation_allowed_paraphrase_only`（2018 艺考专访，粉丝剪辑、单来源）：引用请转述、勿逐字长引。
- 微博小号条目 `verified = false`（single-source），使用时注意交叉核实。
- 时间范围 2014-09-03 → 2026-10-22；按月/按视频导航见 ../index/。
