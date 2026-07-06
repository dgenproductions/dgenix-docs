# Google Business Profile

Manage your Google Business Profile via your AI assistant. Analyse reviews, publish posts, update opening hours and fetch business info without opening the Google dashboard.

**Requirements:** Growth+ plan, connect a Google account via Connectors

---

## Available actions

| Action | Credit cost | Description |
|---|---|---|
| `profile_info` | 15 cr | Fetch business info (name, address, phone, website) |
| `analyse_reviews` | 50 cr | Get reviews with a sentiment score and summary analysis |
| `create_post` | 25 cr | Write and publish a Google Business post |
| `reply_review` | 20 cr | Draft a professional reply to a specific review |
| `update_hours` | 15 cr | Adjust opening hours (including holidays) |

---

## Connecting

1. Go to **Connectors**
2. Click **Connect** on Google Business Profile
3. Log in with the Google account that has access to your Business Profile
4. Grant permission for `business.manage`

The connection only works if you have a verified Google Business Profile.

---

## Example conversations

**Analyse reviews:**
> "Analyse my Google reviews from the past month"

**Create a post:**
> "Make a Google Business post for our summer promotion this weekend"

**Update opening hours:**
> "Set my opening hours for Boxing Day: closed"

**Reply to a review:**
> "Write a professional reply to the negative review about wait times"

---

## Tips

- Use `analyse_reviews` weekly for a quick view of customer satisfaction
- Google Business posts expire after 7 days, plan regular updates
- After changing opening hours it takes a few minutes for Google to show the update
- The skill only works with verified business locations

---

## Limitations

- Uploading photos is not supported (Google API limitation)
- Review replies are final and cannot be deleted via the API
- Maximum 1 location per Google account connection
