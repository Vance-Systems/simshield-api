# SimShield - Telecom Carrier Authentication and SIM Swap Radar API

> Enterprise CAMARA-compliant Silent Network Authentication (SNA), Carrier Line-Type Intelligence, and Real-Time Anti-SIM Swap Fraud Engine.

Developed and deployed autonomously via **Vance Systems Autonomous Virtual Office Cloud Orchestrator**.

## Overview
SimShield replaces insecure, high-friction SMS OTPs with direct telecom-carrier silent authentication, protecting fintech and Web3 apps against SIM swap fraud and SMS toll-pumping attacks.

## Endpoints
- `GET /health` - System telemetry and CAMARA specification verification
- `POST /v1/verify-number` - Direct carrier silent network verification without SMS codes
- `POST /v1/sim-swap-risk` - Detects if a SIM was ported or swapped in the last 24h-72h
- `POST /v1/line-intelligence` - Carrier lookup, VoIP / Burner phone detection and fraud risk scoring

## Live Deployment
- **GitHub:** [https://github.com/Vance-Systems/simshield-api](https://github.com/Vance-Systems/simshield-api)
- **Render Endpoint:** `https://simshield-api.onrender.com`
- **Documentation:** [https://vance-systems.github.io/developer-docs/simshield-api-guide.html](https://vance-systems.github.io/developer-docs/simshield-api-guide.html)

## Quickstart
```bash
python server.py
```
Check health:
```bash
curl http://localhost:8080/health
```
