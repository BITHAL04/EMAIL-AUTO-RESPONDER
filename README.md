# 📧 Automated Email Reply System

The **Automated Email Reply System** is a Node.js application that streamlines email management by **automating responses** to incoming Gmail messages and organizing your inbox with **custom labels**.

---

## 🚀 Key Features

- 🔐 **Authorization Flow**: Initiates OAuth2 flow for Gmail API access via a user-friendly URL prompt.
- 🏷️ **Label Management**: Creates a label `AUTO_REPLIED_MAILS` to mark auto-replied emails.
- ✉️ **Email Processing & Reply**: Fetches unread emails, sends custom replies, and labels them to avoid duplicate responses.

---

## 🛠️ Technologies Used

- **Node.js** – Runtime environment for the backend.
- **[googleapis](https://www.npmjs.com/package/googleapis)** – Google API client library for Node.js.
- **[@google-cloud/local-auth](https://www.npmjs.com/package/@google-cloud/local-auth)** – Simplifies OAuth2 authentication.
- **[node-cron](https://www.npmjs.com/package/node-cron)** – For scheduling periodic inbox checks.
- **FS (File System)** – Manages token storage and reading/writing credentials.
- **Readline** – Captures input from the terminal during the OAuth flow.

---

## ✅ Prerequisites

Before running the app, ensure you have:

- Node.js (v14 or higher)
- Gmail API credentials (`credentials.json`) from Google Cloud Console

---



🏷️ Label Creation
Automatically creates a label AUTO_REPLIED_MAILS if it doesn’t exist.

🤖 Email Auto-Replies
Periodically scans your inbox using node-cron.

Sends auto-generated replies to unread emails.

Labels them to prevent duplicate responses.
