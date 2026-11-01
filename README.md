# SearchAgent

**Agent-as-a-Service for retrieval and discovery.**

SearchAgent turns noisy queries into grounded, ranked answers across changing catalogs, documents, and live sources.

面向动态数据源的搜索 Agent：完成查询理解、混合召回、重排、证据聚合与答案生成。

**Status:** Project scaffold · [Portfolio](https://0x0addc001.github.io/#use-cases)

## Agent loop

| Stage | Responsibility |
|---|---|
| Data | Queries, catalogs, pages, documents, freshness metadata |
| Models | Query rewriting, hybrid retrieval, reranking, grounded synthesis |
| Training | Preference pairs, relevance judgments, reward modeling |
| Inference | Low-latency recall, filtering, reranking, streaming answers |
| Harness | Search APIs, index refreshes, policy and freshness tools |
| Eval | Relevance, coverage, citation quality, latency, zero-result rate |

## Initial scope

- Define a source-independent retrieval contract.
- Support lexical, dense, and hybrid recall.
- Keep citations and source freshness on every answer.
- Expose traceable query rewriting and ranking decisions.

## Roadmap

- [ ] Benchmark adapter and evaluation dataset
- [ ] Hybrid retrieval baseline
- [ ] Agentic query planner
- [ ] Online relevance feedback
- [ ] Production tracing and cost controls

## Engineering principles

- Ground every claim in retrieved evidence.
- Optimize end-to-end task success, not retrieval scores alone.
- Treat freshness, latency, and safety as first-class metrics.

