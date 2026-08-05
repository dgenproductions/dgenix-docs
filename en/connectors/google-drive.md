# Connect Google Drive

The Google Drive connector gives GENI access to your files, so it can find, read and summarise documents and tidy up folders without you opening Drive.

## What you can do with it

| What GENI does | Example |
|---|---|
| Find files | "Find the Van Dijk contract" |
| Read and summarise documents | "Summarise the project plan in my Drive" |
| Create folders | "Create a folder called Quotes 2026" |
| Move files | "Put this file in the Clients folder" |
| Share files | "Share this document with jan@company.com" |

The connection activates the **[Google Drive skill](../skills/google-drive.md)**, available from Starter.

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Google Drive
3. Sign in with the Google account whose files you want to use
4. Grant dGENIX the requested permissions
5. The window closes by itself and the connection is live

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| Read Drive files | Finding, opening and summarising |
| Manage Drive files | Creating folders, moving and sharing files |

This is broad access: GENI can reach every file on the connected account. It
**never deletes** a file, and sharing only happens on your explicit request.

## Checking that it works

Right after connecting, ask GENI:

```
Search my Drive for files with "quote" in the name
```

You get a list of file names and locations. If it stays empty while you do have
such files, the wrong Google account is connected.

## Limits

- GENI never deletes files or folders
- Sharing only happens when you explicitly ask
- It only sees files on the connected account, plus what is shared with it
- Very large files are read partially; ask for a specific chapter or tab

## Troubleshooting

**Connection fails.** Check that you are signed in to the right Google account and try again.

**GENI cannot find a file.** The file lives in another Drive or is not shared with the connected account. Check who owns the file.

**Sharing does not work.** The file sits on a shared drive that blocks external sharing. That is a Google setting, not a dGENIX one.

## Disconnecting

Go to **Dashboard -> Connectors**, click Google Drive and choose **Disconnect**.
You can also revoke access at Google itself via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Frequently asked questions

**Is this the same connection as Gmail?**
No, they are separate connectors. You connect them individually, even for the same Google account.

**Can GENI work in shared drives?**
Yes, if the connected account has access to that shared drive.

**Does dGENIX read all my files?**
Only what your request needs. Nothing is scanned or indexed automatically unless you ask.

---

Back to [Connectors overview](README.md)
See also: [Google Drive skill](../skills/google-drive.md)
On the site: [all integrations](https://dgenix.com/integrations) · [all skills](https://dgenix.com/skills)

*dGENIX Docs, Connect Google Drive, updated August 2026*
