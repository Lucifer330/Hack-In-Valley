# Hack in Valley 2027

Official landing page for Hack in Valley 2027, a hackathon organised by Nerds Room.

## Overview

Hack in Valley 2027 is a multi-stage hackathon bringing together students, developers, designers, founders, and early-stage builders. Shortlisted teams advance through online rounds to an offline grand finale in Himachal Pradesh in January 2027. Event planning is in progress, with registrations opening in the last week of November 2026.

## Live Demo

Live site: <add deployed URL>

## Features

- **Animated Mountain Hero:** Canvas-based procedural Himalayan ridgelines with mouse parallax and drifting node network.
- **Sticky Navigation Bar:** Topbar with dynamic scroll-progress indicator, active section tracking, and mobile drawer menu.
- **Proposed Tracks:** Interactive list of five proposed hackathon tracks.
- **Tentative Timeline ("The Ascent"):** Vertical milestone rail showing progression from Base Camp to Celebration.
- **"Find Your Track" Guide:** Interactive matcher suggesting tracks and team mixes based on interests and role.
- **"Score Your Idea" Tool:** Self-check project evaluation slider tool using the proposed judging criteria weights.
- **Mentors and Judges:** Role profile cards with tentative "Coming Soon" placeholders.
- **Prizes:** Overview of rewards and recognition, with the prize pool marked as To Be Announced.
- **Grand Finale Schedule:** Illustrative one-day offline finale agenda.
- **FAQ:** Accordion answering common questions on registration, eligibility, format, and logistics.
- **Sponsors and Community Partners:** Dedicated, separate sections with empty-state notices and planned category tags.
- **Responsive Design:** Dark-theme layout optimized for mobile, tablet, and desktop viewports without external frameworks.

## Tech Stack

- **HTML5:** Semantic markup with embedded SVG assets.
- **CSS3:** Custom properties, CSS Grid, Flexbox, and responsive media queries. No UI framework.
- **Vanilla JavaScript:** ES5/ES6 DOM manipulation, Canvas 2D API, and event listeners. No runtime dependencies.
- **Google Fonts:** Sora (display) and Inter (body).

## Project Structure

```
.
├── .gitignore
├── README.md
└── index.html
```

## Getting Started

To run the site locally:

1. Open `index.html` directly in any modern web browser.
2. Alternatively, serve the project folder using any local HTTP server:

```bash
npx serve .
```

## Deployment

The website is a self-contained static page with inline assets. It can be hosted at any domain, subdomain, or subpath:

- **Vercel / Netlify:** Import the repository, select framework preset "Other", leave the build command blank, and set the output directory to `.`.
- **GitHub Pages:** In repository Settings > Pages, select deployment from the `main` branch and `/ (root)` folder.

## Updating Content

All site content is configured via JavaScript variables at the bottom of `index.html`. Brand colors are defined in `:root` CSS variables (`--bg`, `--surface`, `--surface-2`, `--line`, `--fg`, `--muted`, `--blue`, `--violet`, `--ice`, `--lime`) at the top of the `<style>` block.

| Target | Variable / Location | Format / Structure |
|---|---|---|
| Registration URL | `CONFIG.registrationUrl` | String (live URL enables registration buttons) |
| Sponsors | `CONFIG.sponsors` | Array of objects: `{name, category, description, url, logo}` |
| Community Partners | `CONFIG.communityPartners` | Array of objects: `{name, region, description, url, logo}` |
| Tracks | `TRACKS` | Array of pairs: `[title, description]` |
| Event Timeline | `TIMELINE` | Array of tuples: `[stage, dateRange, detail, isFinale]` |
| Mentors | `MENTORS` | Array of strings: role descriptions |
| Judges | `JUDGES` | Array of strings: role descriptions |
| Judging Criteria | `CRITERIA` | Array of pairs: `[criterionName, weightPercentage]` |
| Schedule | `SCHEDULE` | Array of pairs: `[timeSlot, activity]` |
| FAQs | `FAQ` | Array of pairs: `[question, answer]` |

## Rules from the Brief

- Use "Tentative", "Proposed", "Coming Soon", and "To Be Announced" labels for unconfirmed details.
- Do not invent mentor or judge names, photos, or affiliations before confirmation.
- Keep Sponsors and Community Partners in distinct sections; empty states show "announcements coming soon".
- Do not display a live countdown timer until the exact finale date and timezone are confirmed.
- Keep the registration button disabled until `CONFIG.registrationUrl` is populated.

## Pending Information

The following items are pending confirmation:
- Exact grand finale dates and venue in Himachal Pradesh.
- Live registration form URL.
- Official problem statements and challenge briefs.
- Final prize pool breakdown and category awards.
- Confirmed mentors and judging panel members.
- Confirmed sponsors and community partner rosters.
- Travel, accommodation, and food details for finalist teams.

## Contact

- **Website:** [nerdsroom.org](https://nerdsroom.org)
- **Email:** [nerdsroomcommunity@gmail.com](mailto:nerdsroomcommunity@gmail.com)
- **LinkedIn:** [Nerds Room](https://www.linkedin.com/company/nerds-room/)
- **Instagram:** [@nerds.room](https://www.instagram.com/nerds.room/)

## Credits and Licence Note

Organised by Nerds Room. Logo and brand assets belong to Nerds Room.
