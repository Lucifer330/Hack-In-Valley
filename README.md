# Hack in Valley 2027: Website

Landing page for **Hack in Valley 2027**, a hackathon organised by [Nerds Room](https://nerdsroom.org).
Built from the official *Website Content & Design Brief*. Single-file site (HTML, CSS, JS). No build step.

## Run locally
Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy
- **Vercel / Netlify:** import this repo, framework preset "Other", no build command, output directory `.`
- **GitHub Pages:** Settings, Pages, deploy from branch `main`, folder `/ (root)`

## Editing content
All content is in the `<script>` block at the bottom of `index.html`.

| What | Where |
|---|---|
| Turn on the Register button | `CONFIG.registrationUrl` (set the live URL) |
| Add sponsors | `CONFIG.sponsors`: `{name, category, description, url, logo}` |
| Add community partners | `CONFIG.communityPartners`: `{name, region, description, url, logo}` |
| Tracks, timeline, FAQs, criteria, schedule | `TRACKS`, `TIMELINE`, `FAQ`, `CRITERIA`, `SCHEDULE` |
| Mentors and judges | `MENTORS`, `JUDGES` (role placeholders until confirmed) |

## Brief rules followed
- Tentative / Proposed / Coming Soon / To Be Announced labels wherever details are not final.
- No invented mentor or judge names, photos or affiliations.
- Sponsors and community partners are separate sections; empty ones show an "announcements coming soon" note.
- No live countdown until the exact finale date and timezone are confirmed.
- Registration button is disabled until `CONFIG.registrationUrl` is set.

## Still pending (from the brief)
Exact finale date, venue, registration URL, official problem statements, prize pool, confirmed mentors/judges, sponsors, community partners, accommodation and travel details.

## Hosting under a subpath
All assets are inline, so the page works at any path (for example `/hack-in-valley/`) or on a subdomain without changes.
