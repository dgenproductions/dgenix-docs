# Connect Slack

Connect your Slack workspace to send messages, read channels, send direct messages and more via your AI assistant.

---

## Steps

1. Go to **Dashboard -> Connectors**
2. Click **"Connect"** on Slack
3. You are redirected to the Slack authorisation screen
4. Select the workspace you want to connect
5. Click **"Allow"**
6. After approval Slack shows as **Connected**

---

## Which skills does this unlock?

- **Slack**, send/read messages, DMs, search, create channels, react

---

## Permissions

dGENIX requests the following Slack scopes:

| Scope | For |
|---|---|
| `channels:read` + `channels:history` | Read public channels |
| `groups:read` + `groups:history` | Read private channels |
| `chat:write` | Send messages |
| `im:read` + `im:write` | Read and send direct messages |
| `files:read` + `files:write` | Fetch and upload files |
| `search:read` | Search messages |
| `reactions:write` | React to messages |
| `channels:manage` | Create channels |
| `users:read` | Read the member list |

---

## Removing the connection

Go to **Dashboard -> Connectors** -> click Slack -> **"Disconnect"**. You can also revoke it via *Slack -> Apps -> dGENIX -> Remove app*.

---

Back to [Connectors overview](README.md)
