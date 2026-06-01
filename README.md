# 🩺 AI Ambient Scribe

> An AI-powered clinical documentation platform built for European hospitals — GDPR-compliant, EHR-integrated, and designed to give doctors their time back.

---

## The Problem

Physicians across Germany and Europe spend more time on paperwork than with patients. The average doctor loses **3.1 hours per day** to documentation and EHR data entry. Burnout rates are at record levels — and administrative overhead is the primary cause.

This project addresses that gap directly.

---

## What It Does

The AI Ambient Scribe listens to doctor-patient conversations in real time, transcribes them, and auto-generates structured clinical notes that write directly into the hospital's existing EHR system. The physician reads, edits if needed, and approves in under 30 seconds.

```
Audio input → Whisper transcription → LLM structuring → EHR write-back → Doctor review
```

No wearables. No new hardware. No workflow disruption.

---

## Key Features

- **Real-time transcription** using a GDPR-compliant EU-hosted or on-premise Whisper pipeline
- **LLM-powered note structuring** that extracts clinical intent and formats it as a proper consultation note
- **EHR write-back** via FHIR API, targeting the top EHR systems used in German hospitals
- **Doctor review UI** — clean web and tablet interface for fast approval or editing
- **GDPR-native architecture** — no patient data ever leaves the EU; full data processing agreement support built in

---

## Project Roadmap

| Stage | Timeline | Goal |
|-------|----------|------|
| **Discovery** | Months 0–1 | 10+ doctor interviews, GDPR path defined, EHR shortlist confirmed |
| **Prototype** | Months 2–4 | Working demo with real EHR write-back, medical advisor sign-off |
| **Pilot** | Months 5–8 | 1–2 paying hospital pilots, time savings documented |
| **Scale** | Months 9–18 | EUR 50K+ MRR, hospital group contracts, CE marking initiated |

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Transcription | OpenAI Whisper (EU-hosted / on-premise) |
| LLM structuring | Claude / GPT-4 via API |
| EHR integration | FHIR R4 API |
| Backend | Python (FastAPI) |
| Frontend | React |
| Infrastructure | Docker, EU cloud (AWS Frankfurt / Azure Germany) |
| Auth & compliance | OAuth 2.0, end-to-end encryption, GDPR DPA support |

---

## Business Model

Per-doctor monthly SaaS subscription, licensed at the hospital department level.

| Segment | Price |
|---------|-------|
| Pilot (flat fee, up to 5 doctors) | EUR 2,000–3,000 / 3 months |
| 1–10 doctors | EUR 180 / doctor / month |
| 11–30 doctors | EUR 140 / doctor / month |
| 30+ doctors | Custom enterprise contract |

**ROI for hospitals:** at EUR 100/hr physician cost and 3.1 hrs/day saved, the product delivers ~50x return on investment per doctor per month.

---

## Why Europe, Why Now

- No dominant GDPR-native AI scribe player exists in the German market yet
- US competitors (DAX Copilot, Suki AI) cannot meet EU data residency requirements without full infrastructure restructuring
- The EU AI Act and tightening GDPR enforcement make compliance-first architecture a durable moat
- German hospitals are significantly underdigitised relative to GDP — the gap is real and the timing is right

---

## Getting Started

> ⚠️ This project is currently in active development. The prototype phase begins in Q3 2026.

```bash
# Clone the repo
git clone https://github.com/your-username/ai-ambient-scribe.git
cd ai-ambient-scribe

# Install dependencies
pip install -r requirements.txt

# Run locally
uvicorn main:app --reload
```

Environment variables required — see `.env.example` for the full list.

---

## GDPR & Compliance

This project is built GDPR-compliant from the ground up:

- All audio processing happens within EU infrastructure
- Patient data is never used for model training without explicit written consent
- Full Data Processing Agreement (DPA) template available for hospital pilots
- Data retention policies, deletion procedures, and audit logging are built into the core architecture

---

## Contributing

This is an early-stage project. If you're a clinician, healthcare IT specialist, or developer interested in contributing — open an issue or reach out directly.

---

## License

MIT License — see [LICENSE](LICENSE) for details.

---

*Built by a software engineer who believes the best healthcare technology is invisible — it just gets out of the doctor's way.*
