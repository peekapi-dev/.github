<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/peekapi-dev/.github/main/profile/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/peekapi-dev/.github/main/profile/banner-light.svg">
  <img alt="PeekAPI — Drop-in API analytics" src="https://raw.githubusercontent.com/peekapi-dev/.github/main/profile/banner-dark.svg" width="100%">
</picture>

<p align="center">
  <strong>Drop-in API analytics for any REST API.</strong><br>
  One middleware. Zero dependencies. Real-time insights.
</p>

<p align="center">
  <a href="https://peekapi.dev">Website</a> ·
  <a href="https://peekapi.dev/signup">Get Started</a> ·
  <a href="https://github.com/peekapi-dev/community/issues/new/choose">Feedback</a>
</p>

---

### What is PeekAPI?

PeekAPI captures HTTP request metadata from your API — method, path, status, latency, consumer — and turns it into a real-time analytics dashboard with smart alerting. Add one line of middleware, get instant visibility.

### SDKs

| Language | Package | Frameworks |
|----------|---------|------------|
| **Node.js** | [`sdk-node`](https://github.com/peekapi-dev/sdk-node) | Express · Fastify · Koa · Hapi · NestJS |
| **Python** | [`sdk-python`](https://github.com/peekapi-dev/sdk-python) | ASGI · WSGI · Django |
| **Go** | [`sdk-go`](https://github.com/peekapi-dev/sdk-go) | net/http · Gin · Echo · Fiber · Chi |
| **Rust** | [`sdk-rust`](https://github.com/peekapi-dev/sdk-rust) | Actix Web · Axum · Rocket |
| **Ruby** | [`sdk-ruby`](https://github.com/peekapi-dev/sdk-ruby) | Rack · Rails |
| **PHP** | [`sdk-php`](https://github.com/peekapi-dev/sdk-php) | PSR-15 · Laravel |
| **Java** | [`sdk-java`](https://github.com/peekapi-dev/sdk-java) | Spring Boot · Jakarta Servlet |
| **Dart** | [`sdk-dart`](https://github.com/peekapi-dev/sdk-dart) | Shelf |

Every SDK is **zero-dependency** — standard library only.

### Quick start

```javascript
// Node.js — that's it
const { peekapi } = require("@peekapi/sdk-node");
app.use(peekapi({ apiKey: "ak_live_..." }));
```

```python
# Python
from peekapi.middleware.asgi import PeekApiASGI
app.add_middleware(PeekApiASGI, api_key="ak_live_...")
```

```go
// Go
client, _ := peekapi.New(peekapi.Options{APIKey: "ak_live_..."})
handler := peekapi.Middleware(client)(mux)
```

### Why PeekAPI?

- **2 minutes to integrate** — no agents, no sidecars, no config files
- **8 languages, 19+ frameworks** — same dashboard, any stack
- **Zero runtime deps** — every SDK uses only the standard library
- **Real-time** — live request stream, not batch analytics
- **Smart alerts** — error rate, latency spikes, usage anomalies, inactivity
- **Privacy-first** — auth headers are SHA-256 hashed, never stored raw

---

<p align="center">
  <a href="https://github.com/peekapi-dev/community/issues/new/choose">Report a bug</a> ·
  <a href="https://github.com/peekapi-dev/community/discussions">Discussions</a>
</p>
