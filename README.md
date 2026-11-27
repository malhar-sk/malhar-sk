### Hi, I'm Malhar

I'm a third-year Computer Science student in Pune, working my way into systems engineering and quality assurance.
My way of learning is to build the kind of systems that need testing most right now (AI agents, payment pipelines,
device fleets) and then try to open them up and see how they tick. Every project here comes with its tests, its numbers, and an honest
note about what I haven't verified.

## What I've been building

**[Multilingual voice agent](https://github.com/malhar-sk/fleet-voice-agent)**: how do you test an AI that listens
and talks back in English, Hindi and Marathi? I wrote 18 Playwright end-to-end tests that play synthetic speech into a
real browser as the microphone. They found 3 bugs, all on the unhappy paths: silence, a dead backend, a dashboard
starved of memory. The agent itself picks the right tool for 96.7% of spoken questions.

**SupplyWatch, the [API](https://github.com/malhar-sk/supplywatch) and its [AI copilot](https://github.com/malhar-sk/supplywatch-copilot)**:
it started as practice with the classic testing stack, 5 test layers on one API plus a load test with 50 virtual
users. Then I put an AI copilot on top and asked whether its answers were actually better, or only looked better.
Retrieval hit@5 went from 0.95 to 1.00 on a 50-question golden set, and re-running the evaluation showed that one
"improvement" was just noise.

**SWIFT payments, a [monitor](https://github.com/malhar-sk/swift-mt103-monitor) and a [message reader](https://github.com/malhar-sk/mt103-extractor-lora)**:
a Go agent on a Raspberry Pi watches simulated payment messages and alerts when one misses its 5-second SLA. Then a
small fine-tuned model reads messy payment text. My first version scored 94.2% but fell to 66.7% on formats it had
never seen, because it was reading fields by position. Retraining on more varied data took it to 99.3% (level with
Claude Haiku) and 89.1% on the unseen formats.

**[Fleet health monitor](https://github.com/malhar-sk/fleet-health-monitor)**: one command turns a laptop or a
Raspberry Pi into a monitoring server that shows every device as online or offline and raises an alert when one goes
quiet. 400 unit tests run in CI.

## Tools I reach for

- **Testing:** Playwright, Selenium, pytest, REST Assured, Postman, k6, GitHub Actions
- **AI evaluation:** RAGAS, golden test sets, out-of-distribution tests, LoRA fine-tuning
- **Systems:** OpenTelemetry, Grafana, VictoriaMetrics, Kafka, Docker, Linux
- **Languages:** Python, TypeScript, Go, Java, SQL

All project data is synthetic or public, and each README says which.

I'm looking for internships in QA, SDET and systems engineering. Say hello on
[LinkedIn](https://www.linkedin.com/in/malhar-satishkumar-29b5972b4).
