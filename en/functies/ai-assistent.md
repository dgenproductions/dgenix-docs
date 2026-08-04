# AI Assistant

The AI Assistant page is the web interface of your personal assistant, GENI. Besides Telegram you can send and receive messages straight from the browser here.

---

## Web chat

Send commands and questions via the input field at the bottom. If you have the Telegram add-on active, messages are synced, you see conversations across both channels.

**Start a new session:** click "New chat" to begin a new conversation. Earlier conversations are kept in the history.

---

## Choosing a model (Growth & Pro)

Above the input field are model buttons. Pick the model that fits your task:

| Model | Speed | Good for |
|-------|-------|----------|
| **Auto** |, | Default, dGENIX picks per task |
| **Haiku** | Fast | Simple questions, short tasks |
| **Sonnet** | Powerful | Writing, analysis, complex tasks |

Auto is available on all plans. Manual model selection requires Growth or Pro. Credits are charged per the model and length of the message (see [The credit system](../hoe-het-werkt/credits.md)).

---

## Side panel, Conversations & Knowledge base

The side panel has two tabs:

### Conversations
- Recent sessions shown by date
- Click a session to load its history
- Delete sessions via the trash icon

### Knowledge base
- Upload files the assistant uses as context
- Supported formats: PDF, Word (.docx), images (JPG, PNG, WebP)
- The assistant reads the content and uses it in its answer

---

## Knowledge document

Your personal knowledge document (created during the intake) is shown as a collapsed accordion. Click the header to expand and read it.

- **Edit:** adjust the document via the "Edit" button
- **Download:** save it as a text file via the "Download" button

The knowledge document is always loaded automatically as context.

---

## Context per project

When you chat inside a **project folder**, the assistant combines two sources:

1. **Global knowledge document**, your personal info, way of working and preferences (always present)
2. **Project instructions**, the specific context of that project (client, tone, rules)

Set project instructions via the gear icon on a project folder in the sidebar. Conversations outside a project only use the global knowledge document.

**Result:** a conversation in project "De Krent Bakery" automatically uses a formal tone and brand guidelines, without repeating it each time.

---

## Voice Chat, speak and listen back

Click the **microphone icon** to the right of the input field. GENI listens, transcribes your question automatically and not only replies in text, it also reads the answer aloud in the voice you set.

**How it works:**

1. Click the mic in the chat, recording starts
2. Ask your question or give a command
3. Click again to stop
4. GENI transcribes -> processes -> streams a text answer -> plays it as speech

**Setting a voice:** go to **Settings -> Assistant -> Voice**. dGENIX uses realistic ElevenLabs voices, with separate Dutch and English voices (a sensible default is set per language). There is also a full **Voice Call** mode (the sound-waves icon) for a hands-free spoken conversation with an animated orb screen.

Voice answers use more credits than text (text-to-speech is charged per characters spoken). Voice messages via Telegram are also processed: GENI transcribes them automatically and replies.

---

## Uploading files for the assistant

Via the paperclip icon in the input field you can attach files to your message:
- Images -> the assistant views and describes them
- PDF/Word -> the assistant reads the content

## Camera in the chat

Click the **+** button to the left of the input field and choose **Camera / Selfie** to take a photo without leaving the chat. A live preview opens; the centre button takes the photo, the arrow button switches between front and back camera. After taking it you can retake or confirm; the confirmed photo is attached to your next message. Works on desktop (webcam) and mobile. Your browser asks for camera permission on first use.

## Personalised suggestions on the empty chat screen

When you open a new conversation you see 6 suggestion cards. Click one to drop the text into your input field, you can still edit before sending. They are chosen based on your plan and your active skills (and surface skills you could still activate). Use the shuffle button for a new set.

## Tools button, modes for deeper answers

Next to the **+** button is a **tools icon**. Click to pick from 5 modes that change how your answer is generated:

| Mode | Plan | What it does |
|---|---|---|
| **Deep Research** | Growth+ | Multi-iteration web search with a numbered source list, ideal for market and competitor analysis |
| **SEO Engine** | Growth+ | Audit of a URL with the top 5 improvements |
| **GEO Engine** | Pro+ | Audit for AI search engines (ChatGPT, Claude, Perplexity) |
| **Step by step** | All plans | Answer in numbered steps, ideal for how-tos |
| **Web search on** | All plans | Force web search for this message, for current info with sources |

An active mode shows an indigo chip above the input field with an x to switch it off. Modes that need a specific skill (Deep Research, SEO/GEO) show an upgrade or activate prompt if you do not have it yet. Sources the assistant uses appear as clickable links below its answer.

---

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "Summarise my unread mail" | Reads your inbox and lists the action items |
| "Find out what this company does" | Researches and returns a summary with sources |
| "Write a quote for this client" | Uses your knowledge document, memory and knowledge base |
| "Analyse my site for visibility" | Starts an audit and explains the outcome |
| "Put this conversation in my workspace" | Saves it as a note or task |

## What you see

You ask for an inbox summary. You do not get a raw list but an ordered answer:

> **12 unread, 3 need action**
>
> - **Sofie van Dijk** , quote approved, wants to sign this week. *Action: send contract.*
> - **Accountant** , VAT return due before the 25th. *Action: supply figures.*
> - **Jan Bakker** , asks whether Thursday's meeting can move.
>
> The other 9 are newsletters and notifications. Shall I archive those?

For an action that changes something or costs money, GENI asks for confirmation
first. You always see the text of an email before it goes out.

## Limits

- **No connection, no access.** GENI only reaches accounts you connected.
- **Irreversible actions always ask for approval**: sending, publishing, scheduling.
- **It never deletes anything.** No mail, no file, no calendar entry.
- **It does not fill in the blanks.** If information is missing, it asks.
- **It does not start on its own.** GENI waits for your instruction or a scheduled task.
- **Model choice and some modes sit in higher plans.** On Free you chat in a limited form.

## Troubleshooting

**It says it cannot reach something.** The connection is missing or expired. Check [Connectors](../connectors/README.md) to see whether the account still shows as Connected.

**The answer is too long or too short.** Adjust your communication style or personal instructions in [Settings](instellingen.md).

**It forgets something from an earlier conversation.** Check your [Memory](geheugen.md); what is not in it, it does not know.

**It uses the wrong client context.** Work in a [project](projecten.md) per client.

**A mode is unavailable.** Deep Research needs Growth, the GEO Engine needs Pro. The chip shows that in advance.

## Frequently asked questions

**Do I have to say which skill it should use?**
No, GENI picks. Steering is allowed: *"use the Social Media Manager to..."*.

**Are my conversations kept?**
Yes, in the side panel. You can organise them into project folders.

**Can it read files I send?**
Yes: images, PDF, Word, Excel, text and audio. See [Files](bestanden.md).

**What does a conversation cost?**
A short question costs little; heavy tasks such as an audit or research cost
more. The cost shows on the button before you start. See
[The credit system](../hoe-het-werkt/credits.md).

---

Next: [Memory](geheugen.md) · [Projects](projecten.md) · [Workspace](werkruimte.md)
On the site: [how dGENIX works](https://dgenix.com/hoe-het-werkt) · [all skills](https://dgenix.com/skills)

*dGENIX Docs, AI assistant, updated August 2026*
