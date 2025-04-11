# Embedded Prompt Injection

## What is it?
This attack involves hiding malicious prompts inside documents, emails, or structured content. When AI systems summarize or interpret such content, they may unknowingly execute the embedded instructions.

---

## Attack Simulation
**Test Content:**
-Last page of the document to summarise-
-<img width="424" alt="Screenshot 2025-04-10 at 10 49 00 PM" src="https://github.com/user-attachments/assets/751908f7-8c84-4279-95a8-4f42bc94383c" />
-Hidden Prompt in the last page of the document to summarise-
- <img width="448" alt="Screenshot 2025-04-10 at 10 49 54 PM" src="https://github.com/user-attachments/assets/abb1ff92-a4db-4398-b123-3b141bcbba95" />


### Platforms Tested:
- Microsoft Copilot
- <img width="941" alt="Screenshot 2025-04-10 at 10 51 00 PM" src="https://github.com/user-attachments/assets/586b21c7-6d4e-4198-b277-5e4755b21b46" />


### Observations:
- AI models embedded in document workflows followed hidden instructions.
- Summarization tools lacked sanitization for injected commands.

---

## Security Risks
- **Document Summarizer Exploits:** Malicious prompts inside HR/finance files.
- **Email Automation Abuse:** AI executes attacker-inserted commands.
- **Internal Tool Manipulation:** Alters AI-generated insights and recommendations.

---

## Mitigations
- **Content Sanitization:** Scan for prompt-like phrases before processing.
- **Context Validation:** Use meta-analysis to flag instruction patterns.
- **Enterprise Controls:** Preprocess documents/emails with threat detection before LLM ingestion.

---

## Takeaway
Structured content isn’t always safe. Treat every input like a potential injection source—especially in enterprise environments.

> "AI doesn’t know the difference between a task and a trap—unless you teach it."
