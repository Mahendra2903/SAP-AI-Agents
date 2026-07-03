# SAP AI Agents

AI-powered automation agents built for mid-market SAP shops 
(SAP B1 / ByDesign) using n8n and Google Gemini.

Built by a SAP Consultant with hands-on experience 
in SAP BTP, Integration Suite, Basis and PI/PO migration.

---

## Agents

### 1. Invoice Email Responder 
**Status:** Working demo ✅

**Problem:** AP teams at SAP B1 companies receive 50+ vendor 
emails per day asking about invoice status, payment dates, and 
confirmations. Each one requires a manual SAP lookup and reply — 
wasting 5–10 hours per week.

**Solution:** An AI agent that automatically:
- Reads incoming vendor emails
- Extracts invoice number and query type
- Looks up invoice status in SAP B1
- Drafts a professional reply

**Stack:**
- n8n (workflow orchestration)
- Google Gemini API (AI brain)
- SAP B1 Service Layer (mock data for demo, real API for production)

**How to use:**
1. Import `invoice-email-responder.json` into your n8n instance
2. Add your Google Gemini API key as a credential
3. Update the mock data in the Code node with your SAP B1 data
4. Connect Gmail trigger for production use

---

## Roadmap

- [ ] Sales Order Status Bot
- [ ] Monthly Close Prep Assistant  
- [ ] Real SAP B1 Service Layer integration
- [ ] Claude API swap (production)

---

## About

Built as part of a consulting practice focused on helping 
mid-market SAP shops automate repetitive back-office processes 
using AI agents.

Interested in deploying this for your SAP environment? 
Connect on LinkedIn: [www.linkedin.com/in/mahendrapalle]
