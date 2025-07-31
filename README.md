# AI-Powered Gmail Auto-Responder with Telegram Approval (n8n Workflow)

This project is an end-to-end automation built using [n8n](https://n8n.io/). It connects Gmail, OpenAI (or ChatGPT), and Telegram to automatically:

- Read incoming emails
- Use AI to draft a suggested reply
- Send the AI-drafted message to Telegram
- Allow the user to approve or reject the message before replying

## 🔧 Tools Used

- [n8n](https://n8n.io/) (Self-hosted via Docker)
- Gmail Trigger Node
- OpenAI Chat Node (AI logic)
- Telegram Node (for approvals)
- ngrok (for testing webhooks externally)

## 🧠 Workflow Overview

1. **Gmail Trigger**: Watches for new promotional emails.
2. **AI Agent**: Drafts an appropriate response.
3. **Telegram**: Sends the draft to the user for manual approval.
4. **Response**: (Optional) Sends the reply or archives based on approval.

## 📦 How to Use

- Import `workflow.json` into your local or cloud n8n instance.
- Set up the required credentials:
  - Gmail OAuth2
  - Telegram Bot Token
- Use ngrok or set `WEBHOOK_URL` in Docker to enable Telegram buttons

## 🔐 Security Tip

Never commit your actual bot tokens or Gmail secrets.

## 📸 Demo Screenshot

<img width="1919" height="880" alt="image" src="https://github.com/user-attachments/assets/e8732922-f6ed-4672-a58d-7e64ab05ded9" />


