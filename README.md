### Hi, I'm Malhar

I build AI systems and the infrastructure under them, and I measure them: every project below ships with its
evaluation numbers, its tests in CI, and an honest list of what was not verified.

## Featured projects

| Project | What it is | Measured |
|---|---|---|
| [**mt103-extractor-lora**](https://github.com/malhar-sk/mt103-extractor-lora) | LoRA fine-tuned Qwen2.5-0.5B that turns messy payment text into validated SWIFT MT103 JSON, served on CPU via Ollama | field accuracy 99.1% in-distribution, 89.0% on unseen formats (from 69.5%); runs on 1 CPU |
| [**supplywatch-copilot**](https://github.com/malhar-sk/supplywatch-copilot) | RAG copilot, LangGraph agent and MCP server over a supply-risk API, with signed webhooks to n8n | RAGAS + retrieval evals on a 50-question golden set (hit@5 1.00) |
| [**fleet-voice-agent**](https://github.com/malhar-sk/fleet-voice-agent) | Voice agent in English, Hindi and Marathi that answers questions about a device fleet by calling PromQL tools | tool accuracy 96.7%, p50 voice-to-voice 8.0 s on a 2-vCPU CPU-only box |
| [**fleet-health-monitor**](https://github.com/malhar-sk/fleet-health-monitor) | One-command device health monitoring for Raspberry Pi / Linux fleets: OTel agent, MQTT, check-in URL, offline alerts | 400 unit tests in CI |
| [**swift-mt103-monitor**](https://github.com/malhar-sk/swift-mt103-monitor) | Go agent on a Raspberry Pi 5 simulating an MT103 bus over Kafka, with SLA and duplicate tracking via OpenTelemetry | Go tests + arm64 build in CI |
| [**supplywatch**](https://github.com/malhar-sk/supplywatch) | FastAPI B2B API scoring critical-mineral supply disruption risk, with alerts and digests | Postman/Newman API tests against PostgreSQL in CI |

## What I work with

- **AI:** LoRA fine-tuning (PEFT/TRL), RAG with pgvector, LangGraph, MCP, tool calling, eval design (RAGAS, held-out OOD sets)
- **Infra:** Docker / Podman, VictoriaMetrics, Grafana, OpenTelemetry, Kafka, MQTT, n8n, GitHub Actions
- **Languages:** Python, Go, SQL

All project data is synthetic or public, and each README says which.
