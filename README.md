### Sandeep Kesarwani

Systems architect. I design and operate distributed platforms that process 200B+ data points/month across 750K industrial sensors.

I believe in building from first principles — understanding the machine before writing the code. When Celery’s ETA scheduler had an unbounded memory leak, I didn’t file an issue. I traced it through Kombu’s QoS layer, found the missing prefetch cap, and shipped the fix upstream. It runs in production everywhere now.

---

Currently building:

[StreamGate](https://github.com/sashu2310/streamgate) — Lock-free observability governance proxy in Go. 200K+ events/sec, zero-allocation hot path. Filters noise and redacts PII from observability pipelines before they hit your vendor. Recognized by Datadog engineering.

[Cartograph](https://github.com/sashu2310/cartograph) — AI-powered code flow explorer. Parses codebases, discovers entry points, traces execution flows as interactive DAGs. Don’t read the code — read the story. Tested against a production Django/Celery codebase (509 entry points discovered).

---

Open source contributions:

- Celery — Fixed unbounded memory leak in ETA task scheduling. Shipped in v5.6.0. [PR #9853](https://github.com/celery/celery/pull/9853)
- Kombu — Added max_prefetch to QoS class, capping heap growth. Shipped in v5.6.0. [PR #2348](https://github.com/celery/kombu/pull/2348)

Celery is downloaded 10M+ times/month. The fix affects every deployment using ETA/countdown tasks.

---

What I work with:

Go Python Distributed Systems PostgreSQL TimescaleDB Celery Redis RabbitMQ Kubernetes AWS OpenTelemetry

---

Writing: [musashiforge.hashnode.dev](https://musashiforge.hashnode.dev)

LinkedIn: [sandeep-kesarwani](https://www.linkedin.com/in/sandeep-kesarwani/)
