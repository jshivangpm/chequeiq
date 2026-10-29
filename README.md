# chequeiq
AI-powered cheque image processing — multi-source schema normalisation, AI extraction, confidence thresholds, human-in-the-loop review, and on-us/transit routing.
▶️ **[Watch the 5-min demo on Loom](https://www.loom.com/share/603eb89f83bb479aaf2684db10695fe8)**
📄 **[View the product overview deck](ChequeIQ.pdf)**

## The problem

Banks receive cheque images from many channels — branch scanners, ATMs, mobile deposits, partner banks — each with its own format and metadata. Normalising this data and extracting fields accurately is still heavily manual, slow, and error-prone, and every misread field creates downstream exceptions.

## What ChequeIQ does

- **Multi-source schema normalisation** — maps incoming cheque data from different channels into one standard schema
- **AI extraction** — reads key fields (payee, amount, date, MICR details) from cheque images
- **Confidence thresholds** — auto-approves high-confidence extractions and flags uncertain ones
- **Human-in-the-loop review** — routes low-confidence items to an operator queue for quick verification
- **On-us / transit routing** — identifies whether a cheque is drawn on the same bank or another bank and routes it accordingly

## How it works

1. Cheque images and metadata arrive from multiple sources
2. Data is normalised into a common schema
3. AI extracts fields and assigns confidence scores
4. Items above threshold are processed automatically; the rest go to human review
5. Cleared items are routed as on-us or transit

## Product thinking

- **Precision over automation rate** — thresholds are tuned so that what goes through automatically is trustworthy, rather than maximising straight-through processing at the cost of errors
- **Reviewer efficiency** — the review queue surfaces only the uncertain fields, not the whole cheque
- **Built for real operations** — designed around how bank operations teams actually handle exceptions

## Built with

Prototype built with Claude (Anthropic) as an AI-assisted product exploration.

---

*Built by [Shivang Jindal](https://www.linkedin.com/in/shivang-jindal-pm) — Senior Product Manager, fintech & enterprise SaaS.*
