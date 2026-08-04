# Connecting LinkedIn

The LinkedIn connection lets GENI publish posts on your profile and fetch the statistics of your recent posts.

The connection activates the [LinkedIn skill](../skills/linkedin.md), available
from **Growth**.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "Publish this text on LinkedIn" | Posts text to your profile |
| "Write a post about our new product and get it ready" | Writes the text and asks for approval first |
| "How did my last posts do?" | Fetches views, likes and comments |
| "What is in my profile?" | Reads name, headline and profile photo URL |

Combining it with other skills is where this gets interesting: have GENI turn a
blog article into a LinkedIn post, or condense a weekly report into one update.

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to LinkedIn
3. Log in with your LinkedIn account
4. Grant the requested permissions
5. LinkedIn then shows as **Connected**

## What access you grant

| Scope | What dGENIX uses it for |
|---|---|
| `r_liteprofile` | Reading your name, headline and profile photo |
| `r_emailaddress` | Retrieving your email address |
| `w_member_social` | Publishing posts on your profile |

> **Note:** LinkedIn has to approve the `w_member_social` scope through their
> Developer Program. That can take 1 to 2 weeks. Reading your profile and
> fetching statistics works right after connecting.

## Checking that it works

Ask this right after connecting:

```
What is in my LinkedIn profile?
```

You get your name and headline back. If that works, the reading side is fine.
Whether publishing works depends on the approval above.

## Limits

- Publishing a post **always** asks for confirmation; you read the text first
- Text posts only; images, video and documents are not supported
- Posting to a **company page** is not possible, only to your personal profile
- GENI does not delete or edit existing posts
- Commenting on other people's posts and sending connection requests are not supported

## Troubleshooting

**Publishing returns a permissions error.** The `w_member_social` scope has not been approved yet. Reading already works; publishing becomes available once LinkedIn approves.

**Statistics come back empty.** LinkedIn only supplies figures after a while. For a fresh post that is normal.

**You want to post on your company page.** This connection does not support that. Have GENI write the text and post it yourself.

## Disconnecting

Go to **Dashboard -> Connectors**, click LinkedIn and choose **Disconnect**. In
LinkedIn you can also revoke access via *Settings -> Data privacy -> Other
applications*.

## Frequently asked questions

**Can GENI post automatically every week?**
Yes, through a recurring task. The confirmation still applies, so nothing ever
goes out that you have not seen. See [Scheduled tasks](../handleiding/geplande-taken.md).

**Can GENI see my inbox or connections?**
No. The connection grants no access to messages, connections or your feed.

**Can I set the tone myself?**
Yes. Put how you want to write in your knowledge document or memory and GENI
sticks to it. See [Context storage compared](../concepten/context-opslag-vergeleken.md).

---

Back to [Connectors overview](README.md)
See also: [LinkedIn skill](../skills/linkedin.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting LinkedIn, updated August 2026*
