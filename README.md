
# URL Shortener + Analytics

Production-style backend to practice clean REST design, logging, concurrency, and caching.

**Problem.** Build a small, production-style backend that proves you can ship a clean REST API with correct HTTP semantics, strong validation, structured logging, concurrency where it matters, and a cache you actually measure. The concrete product: a URL Shortener + Analytics microservice.

**Primary users.**

- **Anonymous sharers**: just want a short link that works.

- **Developers**: integrate shortening into apps via an API and monitor usage.

- **Admins**: manage abuse, quotas, and operational health.

**Single success metric (v1).**
p95 redirect latency ≤ 25 ms for cache hits at ≥ 300 RPS on a single node with Redis enabled.
