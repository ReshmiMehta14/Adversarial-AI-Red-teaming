# Crescendo Jailbreak

## What is it?
A crescendo jailbreak is a multi-step attack that gradually coaxes an AI into revealing restricted content by fragmenting the malicious query into benign parts.

---

## Attack Simulation
**Strategy:**
- Break the forbidden question into smaller, less suspicious steps.
- Slowly build up to the restricted content through conversation.

### Platforms Tested:
- DeepSeek AI
- <img width="508" alt="Screenshot 2025-04-10 at 10 40 57 PM" src="https://github.com/user-attachments/assets/47a7bc23-19ce-434c-838b-de2b1d7aa728" />

- Microsoft Copilot
- <img width="366" alt="Screenshot 2025-04-10 at 10 41 35 PM" src="https://github.com/user-attachments/assets/109b392e-0524-4142-b77e-58976498ae86" />
<img width="365" alt="Screenshot 2025-04-10 at 10 41 52 PM" src="https://github.com/user-attachments/assets/8dd9b433-05bb-444c-b22a-57c218ebcfc5" />
<img width="369" alt="Screenshot 2025-04-10 at 10 42 06 PM" src="https://github.com/user-attachments/assets/2d3d788d-2f99-446c-ae34-3a359d90d031" />
<img width="367" alt="Screenshot 2025-04-10 at 10 42 27 PM" src="https://github.com/user-attachments/assets/d58ed896-f30e-4ae4-9d10-f379e7044739" />
<img width="388" alt="Screenshot 2025-04-10 at 10 42 43 PM" src="https://github.com/user-attachments/assets/92e5e7d5-d520-48eb-9a48-943b6f994d11" />
<img width="343" alt="Screenshot 2025-04-10 at 10 42 57 PM" src="https://github.com/user-attachments/assets/33802b7d-ea6d-4a6b-b690-823a26836d93" />



### Observations:
- Context accumulation allowed the AI to reveal restricted content.
- No context-tracking filters detected the multi-turn evasion.

---

## ⚠️ Security Risks
- **Contextual Evasion:** Attacks go undetected in long conversations.
- **Stepwise Leaks:** Sensitive info gets revealed gradually.
- **Bypassing Filters:** AI fails to recognize malicious intent spread across prompts.

---

## 🛡️ Mitigations
- **Context-Aware Filtering:** Track and analyze full conversation threads.
- **Intent Detection Models:** Flag multi-step adversarial behavior.
- **Rate-Limiting Sensitive Topics:** Throttle repetitive queries about restricted content.

---

## 📌 Takeaway
This jailbreak shows that AI safety can’t just evaluate single prompts in isolation. Holistic, conversation-wide security is necessary.

> "Evasion doesn’t always happen in one step. Sometimes it whispers."
