# SoulAssignment
 The POC should demonstrate your ability to lead the development of scalable, ethical ML solutions while considering real-world constraints such as real-time performance, data privacy, and model interpretability.
# AI Safety Chatbot POC

This project is a **proof-of-concept (POC) AI Safety Chatbot** deployed via Google Colab using **Gradio**.  
The chatbot detects **abuse, crisis, escalation, and age-inappropriate content**, and includes **persistent conversation** support.

---

## Features

- **Abuse Detection:** Uses a pre-trained `unitary/toxic-bert` model to identify toxic language.  
- **Crisis Detection:** Detects keywords related to suicidal thoughts or self-harm.  
- **Escalation Detection:** Tracks conversation sentiment to detect negative escalation trends.  
- **Age-Appropriate Filtering:** Blocks messages containing adult content for users under 13.  
- **Persistent Conversation:** Conversation history is stored in `conversation_history.json`.  
- **Web Deployment:** Runs in Google Colab and provides a **public URL** for testing via Gradio.

---

## Dependencies

The project requires the following Python packages:

- `gradio`
- `transformers`
- `torch`
- `textblob`

These are installed in Colab via:

```bash
!pip install gradio transformers torch textblob
Running on public URL: https://xxxx.gradio.app
