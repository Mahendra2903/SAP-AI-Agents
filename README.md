# SAP AI Agents

AI-powered automation agents built for mid-market SAP shops (SAP B1 / ByDesign) using n8n and Google Gemini.

Built by a SAP Consultant with hands-on experience in SAP BTP, Integration Suite, Basis and PI/PO migration.

---

## Agents

### 1. Invoice Email Responder
**Status:** Fully autonomous v2 ✅  
**Stack:** n8n · Google Gemini API · SAP B1 Service Layer (mock) · Gmail

**The problem**

AP teams at SAP B1 companies receive 50+ vendor emails per day asking about invoice status, payment dates, and confirmations. Each one requires a manual SAP lookup and reply — wasting 5–10 hours per week.

**The solution**

A fully autonomous AI agent that watches a Gmail inbox, reads incoming vendor emails, looks up invoice status in SAP B1, and sends a professional reply automatically — all within 60 seconds. Zero human involvement.

**How to use**

1. Import `invoice-email-responder-v2.json` into your n8n instance
2. Connect your Gmail account via OAuth
3. Add your Google Gemini API key as a credential
4. Update the Code node with your SAP B1 data
5. Publish the workflow — it runs automatically from there

**Results**

- Processes vendor emails within 60 seconds of arrival
- Saves AP teams 5–10 hours per week
- Handles payment status, invoice confirmation, and payment date queries

---

## Roadmap

- [x] Invoice Email Responder v1 (manual trigger + mock SAP data)
- [x] Invoice Email Responder v2 (Gmail trigger + auto-reply)
- [ ] Confidence scoring + human review queue
- [ ] Real SAP B1 Service Layer API integration
- [ ] Sales Order Status Bot
- [ ] Monthly Close Prep Assistant
- [ ] Live dashboard UI
- [ ] Claude API swap (production)

---

## Tech Stack

| Layer | Tool |
|---|---|
| Workflow orchestration | n8n (cloud) |
| AI brain | Google Gemini API (free tier) |
| SAP data | SAP B1 Service Layer (mock JSON for demo) |
| Email trigger | Gmail OAuth |
| Production AI | Claude API (planned) |

---

## About

Built as part of a consulting practice focused on helping mid-market SAP shops automate repetitive back-office processes using AI agents.

Interested in deploying this for your SAP B1 environment?  
Connect on LinkedIn: [www.linkedin.com/in/mahendrapalle]
