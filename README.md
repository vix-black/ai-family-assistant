# ai-family-assistant

Claude Project for busy families. Connects your calendar, manages all the invites, updates partners by email, helps you manage your family and relieve the cognitive load.

It reads your calendars and inbox, files nursery and school letters into the calendar, flags clashes early, keeps an eye on how full your week is, and sends a morning brief to you and a weekly summary to your partner.

## Start here

You do four things. The assistant does the rest by asking you questions, one at a time, and writing up your household file as it goes. Allow about 30 minutes; you can stop and pick up later.

### Before you start

- A paid Claude plan (Pro or Max).
- The Claude app on your phone **and** desktop ([claude.ai/download](https://claude.ai/download)). Desktop is easier for setup; your phone is where the brief and reminders land, so turn notifications on.
- Know which mail and calendar you use: Google, Outlook/Hotmail, or something else (iCloud, Yahoo). The assistant will help with the rest.
- Have your nursery or school's term dates and closure days to hand (PDF, link or a photo), plus drop-off and pick-up times.

### Your four steps

1. **Create the Project.** In Claude, go to Projects → New Project. Name it anything, e.g. "Family assistant".
2. **Paste the instructions.** Open *Set project instructions*, paste the whole of [`project-instructions.md`](project-instructions.md), and save. No editing needed.
3. **Start a chat in the Project** and type: **start setup**
4. **Upload the file it gives you.** At the end it hands you `household.md`. Add it to the Project with the **+** button on the Project page. Done.

If you stop halfway, ask for "the file so far", upload it, and say **continue setup** in a new chat.

Moving from ChatGPT? Run [`prompts/chatgpt-migration.md`](prompts/chatgpt-migration.md) there first and paste the result in when setup starts.

## Which mail and calendar?

| You use | Connect | Shared calendar | School documents |
| --- | --- | --- | --- |
| Gmail / Google Calendar | Google Calendar, Gmail, Google Drive | Google calendar called `Family` | Google Drive |
| Outlook, Hotmail, Live or Microsoft 365 | Microsoft 365 | Outlook calendar called `Family` | OneDrive |
| iCloud, Yahoo or other | Google connectors, on a free Google account just for the family | Google calendar called `Family`, added to your phone | Google Drive |

No cloud storage? Skip the folder and upload documents straight into the Project.

## What setup covers

1. Its name, how you like replies, and (optionally) how you work best
2. What counts as time for yourself, and whether to flag when it's squeezed
3. Your mail, calendar and storage — it tests the connections and tells you what to click if one is missing
4. The shared Family calendar
5. The school or nursery folder
6. Both adults' work, including self-employed hours, invoicing and tax deadlines
7. Your partner's sport and social commitments — e.g. a season ticket, with home fixtures looked up and offered for the calendar
8. The children: nursery or school, drop-off and pick-up times, who does each, what goes in the bag, wraparound care, clubs
9. Term dates and closure days
10. House, health, pets, car, family and friends

**You end up with:**

- `household.md` — your household written up (see [`templates/household-template.md`](templates/household-template.md) for what it contains)
- Term dates and closure days in both calendars (after you confirm)
- Your partner's home fixtures in the Family calendar, if they have a season ticket
- Up to three scheduled tasks: morning brief, weekly summary for your partner (drafted, never sent without you), weekly school folder check
- A gentle load check: if your week fills up or there's no time for you, it says so and offers to hold time

**It won't ask for** dates of birth, medical details, ID or bank details. First names and school years are all it needs.

## Privacy

- The children are minors. Their details stay in your own calendars, storage and Claude Project.
- Don't commit your filled-in `household.md` to this or any repo.
- Emails are always drafts for you to review.
- Turn on two-factor authentication on your Google/Microsoft and Claude accounts.

## Files

| File | What it is |
| --- | --- |
| [`project-instructions.md`](project-instructions.md) | Paste into the Claude Project's instructions |
| [`prompts/chatgpt-migration.md`](prompts/chatgpt-migration.md) | Prompt to export your context from ChatGPT |
| [`templates/household-template.md`](templates/household-template.md) | What the household file looks like (setup fills it in for you) |
| [`docs/full-guide.pdf`](docs/full-guide.pdf) | Full reference guide: options, connectors, scheduled tasks, privacy checklist |
