Research on Improving the Quality of Online Customer Support Using Artificial Intelligence

Companies Best Suited for This Solution

## Intercom:
It’s designed around conversational support and live-chat first, with strong APIs and webhook support — ideal for plugging in an LLM + retrieval pipeline as the Smart Support Assistant (SSA) from your thesis.

Your thesis calls for multi-channel ingestion (chat, email, social, CRM), retrieval-augmented generation (RAG), sentiment-aware response generation, and a human-in-the-loop escalation flow — Intercom’s architecture and app marketplace are well suited for that integration pattern. 

MasterThesisReport_RakshithaShy…

MasterThesisReport_RakshithaShy…

For an academic/industry deployment you can prototype quickly with Intercom’s developer tools, then scale to enterprise platforms (Zendesk / Salesforce) if the customer needs deeper ticketing, reporting, or org-wide CRM integration. The thesis explicitly recommends a modular pipeline (preprocessing → intent/sentiment → RAG → LLM → human fallback) — this fits Intercom’s extension model.

## Zendesk: excellent if the organization prioritizes ticketing and agent workflows; integrates well with knowledge base + LLMs.

## Salesforce Service Cloud: enterprise-grade CRM + automation — best if you must tightly integrate with sales/CRM records at scale.
(Use Intercom for fastest prototype and clearer mapping to the SSA pipeline in your thesis; migrate to Zendesk/Salesforce for enterprise rollouts.)
