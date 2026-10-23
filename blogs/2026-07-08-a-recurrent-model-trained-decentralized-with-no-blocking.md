---
title: "A recurrent model trained decentralized, with no blocking and almost no quality loss"
url: "https://chutes.ai/news/non-blocking-recurrent-training"
date: "2026-07-08"
author: "Timon Agar"
feed_url: "https://chutes.ai/news/rss.xml"
---
We trained a pure recurrent model across distributed GPUs with fully non-blocking synchronization, and it landed within 0.6% of the centralized baseline at matched steps. As far as we know, that is the first time decentralized non-blocking training has held up on a recurrent architecture. The tradeoff we set out to break Training a model across many GPUs in different places forces a familiar choice.
