<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg">
  <img src="./assets/banner-light.svg" width="100%" alt="KIDAVI. Lenny Kidavi, developer and product builder, Nairobi.">
</picture>

I'm Lenny, a Computer Science student at the Catholic University of Eastern Africa and a freelance full-stack developer in Nairobi. I design and build web products end to end, from the Figma file to the deployed app, and I'm working toward machine learning engineering.

**[Portfolio](https://kidavi.me)** · [LinkedIn](https://www.linkedin.com/in/lenny-kidavi-4693ba355) · [Email](mailto:lennykidavik@gmail.com) · [Fiverr](https://www.fiverr.com/lennynavwani) · [X](https://x.com/Lenny_kidavi) · [CV](https://kidavi.me/cv)

<sub>Jump to: [Now](#now) · [Selected work](#selected-work) · [Being built](#being-built) · [Recognition](#recognition) · [Toolkit](#toolkit) · [Across the sand](#across-the-sand)</sub>

<!--
  NOW: the only section meant to change often.
  Edit the lines and the date. One short line each, four lines max.
-->
## Now

<sub>Updated 26 Nov 2026</sub>

- **Shipped** — [Allenet Bakers](https://allenetbakers.vercel.app): full rebrand and website for a custom-cake bakery
- **Launching** — [Saka](https://sakahapa.app) in a soft launch with professionals first, and building its Android app
- **Relaunched** — [Akibora](https://www.smartchama.tech), SmartChama rebuilt for web and Android on one database
- **Building** — two client products, Atrium and Planwright
- **Studying** — for December exams: AI, statistics, computer architecture, OOP and cloud computing

## Selected work

<sub>Click a picture to open the live site. Open <b>Case notes</b> for the story behind each one.</sub>

<!--
  Cards: two per row. Copy a <td> block to add one. Keep the one-line
  description under ~15 words; longer text goes inside <details>.
  Thumbnails live in assets/work/ (1200x750, 16:10).
-->

<table>
<tr>
<td width="50%" valign="top">

<a href="https://sakahapa.app"><img src="./assets/work/saka.jpg" width="100%" alt="Saka marketplace home page"></a>

### Saka
<sub>Product · Founder · Soft launch</sub>

Inquiry-first marketplace for trusted local professionals and businesses in Nairobi. Direct M-Pesa, no commission.

<sub>Next.js 14 · Supabase · PostGIS · MapLibre · Cloudinary · Android (TWA)</sub><br>
[Live](https://sakahapa.app) · Private repo

<details>
<summary><b>Case notes</b></summary>
<br>

Finding a plumber, electrician, salon or mechanic you can trust in Nairobi usually means asking around. On Saka you message a provider directly, agree on the job, and pay them straight through M-Pesa; Saka takes no commission. I'm the main founder and lead product in a team of five.

- Database rebuilt from scratch in Nov 2026, with the trust rules enforced in Postgres: nobody can verify themselves or edit their own ratings, and reviews only follow completed jobs
- Free OpenStreetMap maps, and locations rounded to about 1 km for privacy
- A 1–2 MB Android app on the same database as the website, for phones with little storage

**Hardest part:** finding skilled providers and checking them before they're approved, because the marketplace is only as good as the people on it.
</details>

</td>
<td width="50%" valign="top">

<a href="https://www.smartchama.tech"><img src="./assets/work/smart-chama.jpg" width="100%" alt="Akibora home page: Every shilling your chama saves, kept in the open"></a>

### Akibora <sub>(formerly SmartChama)</sub>
<sub>Product · 2026 · Hackathon winner · Early access</sub>

Chama savings over M-Pesa: merry-go-round, welfare, loans and a credit passport, all in the open.

<sub>Next.js 16 · React 19 · Supabase · M-Pesa Daraja · Expo · Solidity</sub><br>
[Live](https://www.smartchama.tech) · [Code](https://github.com/chillyreward/SmartChama)

<details>
<summary><b>Case notes</b></summary>
<br>

Chamas run on trust, but most still track contributions, loans and Merry-Go-Round turns in notebooks and WhatsApp threads. My team and I built SmartChama to make that automatic and visible: M-Pesa contributions are tracked as they come in, loans and rotation schedules live in one place, and a Solidity smart-contract layer records the group's rules so no single person can quietly change them.

**Hardest part:** the M-Pesa integration. Members now pay with an STK push and see it in the group's records as it happens.

**Recognition:** 1st place at Red, White & Build (U.S. Embassy Kenya), 2nd at Beorchild. Built with Rachael, Shilla and Nanjoli.

**Now:** relaunched as **Akibora**, with the web and Android apps rebuilt from scratch on one shared, locked-down database. Members' on-time payments build a trust score they can download as a credit passport. Automatic M-Pesa payouts and SmartGrow aren't open yet.
</details>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://dogear-nine.vercel.app"><img src="./assets/work/dogear.jpg" width="100%" alt="Dogear landing page: Leave the playlist. Keep your place."></a>

### Dogear
<sub>Own product · 2026</sub>

Spotify companion that keeps a fixed shuffle per playlist and resumes on the exact song and second.

<sub>Next.js · TypeScript · Supabase · Spotify Web API · Vercel</sub><br>
[Live](https://dogear-nine.vercel.app) · Private repo

<details>
<summary><b>Case notes</b></summary>
<br>

Switch playlists on Spotify and your shuffle is gone when you come back. Dogear keeps a fixed, seeded shuffle for each playlist and a bookmark where you stopped, so **Resume** lands on the same song, at the same second.

- Shuffle that spreads each artist's songs out evenly, reproducible and unit-tested
- Background polling every ~20 s, with Postgres row locks so two pollers never handle the same user
- Listening insights, skip suggestions, CSV export
- Encrypted refresh tokens and row-level security on every table
- Installable on your phone

<sub>Runs in Spotify's development mode, so it's limited to a handful of invited users.</sub>
</details>

</td>
<td width="50%" valign="top">

<a href="https://allenetbakers.vercel.app"><img src="./assets/work/allenet-bakers.jpg" width="100%" alt="Allenet Bakers home page: Cakes baked for the days you'll remember"></a>

### Allenet Bakers <sup>new</sup>
<sub>Client · Brand and web · 2026</sub>

Rebrand and website for a custom-cake bakery: real cakes, real prices, order on WhatsApp.

<sub>Next.js 16 · React 19 · TypeScript · Tailwind CSS v4</sub><br>
[Live](https://allenetbakers.vercel.app) · Private repo

<details>
<summary><b>Case notes</b></summary>
<br>

My mum's bakery in Ongata Rongai ran almost entirely on WhatsApp and word of mouth, and customers had to ask for every price. I redrew the logo, built a blush-and-chocolate brand around it, and designed and built the site.

- A cake builder: pick flavour, size, finish and extras, watch a drawing of the cake build itself and the estimate add up, then send the order to WhatsApp, already written out
- A price list from the owner's own per-kg prices, also exported as a WhatsApp image and a PDF
- A gallery of real cakes, grouped by occasion

**Decision:** my first version had a database and an admin inbox. I dropped both, because orders already live in WhatsApp. The site is now fully static and every price lives in one file.
</details>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://gikuyu-translate.vercel.app"><img src="./assets/work/gikuyu-translator.jpg" width="100%" alt="Gikuyu Translator interface"></a>

### Gikuyu Translator
<sub>Experiment · 2026</sub>

AI translation from English and Kiswahili into Gikuyu, with spoken output.

<sub>Next.js · Gemini API · ElevenLabs API</sub><br>
[Live](https://gikuyu-translate.vercel.app) · [Code](https://github.com/chillyreward/New-translator)

<details>
<summary><b>Case notes</b></summary>
<br>

Built for learners, families and communities keeping the language alive. Gemini handles translation, ElevenLabs reads the result aloud, and a phrasebook and history keep useful translations close. Now part of NeuroGrowth's product line.

**Hardest part:** finding an API that handles Gikuyu well enough to be useful.
</details>

</td>
<td width="50%" valign="top">

<a href="https://www.neurogrowthtech.com"><img src="./assets/work/neuro-growth.jpg" width="100%" alt="NeuroGrowth Tech home page: Intelligent systems for ambitious African businesses"></a>

### NeuroGrowth
<sub>Team · Marketing Engineering · 2026</sub>

Full website upgrade for a Nairobi AI engineering studio.

<sub>Next.js · TypeScript · Tailwind CSS</sub><br>
[Live](https://www.neurogrowthtech.com) · [Code](https://github.com/Neuro-growth/neurogrowthwebsite)

<details>
<summary><b>Case notes</b></summary>
<br>

NeuroGrowth Tech builds automation, chatbots and prediction systems for African businesses. I'm on the team in Marketing Engineering and led the upgrade of the company website.
</details>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://oppoliakenya.co.ke"><img src="./assets/work/oppolia.jpg" width="100%" alt="Oppolia Woodworths Kenya home page"></a>

### Oppolia Woodworths Kenya
<sub>Client · 2026</sub>

Showcase and quote-request site for a luxury fitted-cabinetry company.

<sub>Next.js · TypeScript · Tailwind CSS</sub><br>
[Live](https://oppoliakenya.co.ke)

<details>
<summary><b>Case notes</b></summary>
<br>

A showcase for their kitchens and interior work, with clear ways to start a project: request a free quote, talk to a designer, or message the team on WhatsApp. I built it as the full-stack developer.
</details>

</td>
<td width="50%" valign="top">

<a href="https://sucre-bushworks.vercel.app"><img src="./assets/work/sucre-bushworks.jpg" width="100%" alt="Sucre Bushworks home page"></a>

### Sucre Bushworks
<sub>Client · 2026</sub>

Camping gear, Kenyan campsites and guided trips, with an inquiry basket sent over WhatsApp.

<sub>Next.js · TypeScript · Tailwind CSS</sub><br>
[Live](https://sucre-bushworks.vercel.app)

</td>
</tr>
</table>

<sub>And **[this portfolio](https://kidavi.me)** ([code](https://github.com/chillyreward/DunePortfolio)): my site, built on an original design system inspired by Frank Herbert's *Dune*, sand by day and Giedi Prime by night.</sub>

## Being built

<sub>Work in progress. Most of these repositories are private, so they don't show on my profile; <a href="mailto:lennykidavik@gmail.com?subject=Walkthrough%20request">ask me for a walkthrough</a>.</sub>

**Saka for Android** — a 1–2 MB app that opens Saka full-screen and shares the website's database, for phones with little storage.

<table>
<tr>
<td width="50%" valign="top">

<img src="./assets/work/atrium.svg" width="100%" alt="Atrium: survey contour lines around a courtyard plan">

### Atrium
<sub>Client · In progress</sub>

Property advisory web app for a Kenyan client, priced in KES.

<details>
<summary><b>Scope</b></summary>
<br>

- Listings with filters, verification checks and payment-plan illustrations
- Admin with a leads pipeline and an AI lead qualifier that drafts WhatsApp replies
- Client portal: holdings, payment schedules and documents

<sub>Next.js 14 · TypeScript · Tailwind CSS · Supabase</sub>
</details>

</td>
<td width="50%" valign="top">

<img src="./assets/work/planwright.svg" width="100%" alt="Planwright: a floor plan on a millimetre grid">

### Planwright
<sub>Client · In progress</sub>

Browser-based 3D interior design tool for interior designers.

<details>
<summary><b>Scope</b></summary>
<br>

- Precise 2D floor-plan editor, every value in millimetres
- 3D walkthrough generated from the same design document
- Parametric cabinets, drawings and cut lists; AI features in later phases

<sub>Next.js 14 · TypeScript · Supabase · later React Three Fiber</sub>
</details>

</td>
</tr>
</table>

## Recognition

<!-- Newest first. Format: Result — Event, organiser · Month Year · Project -->

<table>
<tr>
<td width="45%" valign="top">
<img src="./assets/work/red-white-build.jpg" width="100%" alt="The winning team holding the $1,000 prize cheque from U.S. Embassy Kenya">
</td>
<td valign="top">

**1st place** — Red, White & Build US–Kenya Hackathon (AI & Tech)<br>
<sub>U.S. Embassy Kenya · Nairobi · 19 Feb 2026 · $1,000 prize</sub>

Won with **SmartChama**, with Rachael, Shilla and Nanjoli.

**2nd place** — Beorchild Hackathon<br>
<sub>Online · 2026</sub>

Second place, again with **SmartChama**.

</td>
</tr>
</table>

## Toolkit

**Ship with** &nbsp; TypeScript · Next.js · React · Tailwind CSS · Supabase · PostgreSQL · Zustand · TanStack Query · Vitest · Playwright · Vercel · Figma<br>
**Also used** &nbsp; Solidity · Firebase · PostGIS · MapLibre · Spotify Web API · Gemini API · Python · Java · C · Docker · Git<br>
**Learning** &nbsp; PyTorch · statistics and probability for ML

## Recent activity

<!--
  Filled in automatically every day by .github/workflows/recent-activity.yml.
  Only public repositories appear here; most client work is private.
  Do not edit between the two markers; the workflow overwrites it.
-->
<!--START_SECTION:activity-->
- [SmartChama](https://github.com/chillyreward/SmartChama) — SmartChama: A PWA digital ledger for Kenyan Chamas built with Next.js and Firebase. <sub>· updated 24 Nov 2026</sub>
- [SmartChama-Mobile](https://github.com/chillyreward/SmartChama-Mobile) <sub>· updated 24 Nov 2026</sub>
- [DunePortfolio](https://github.com/chillyreward/DunePortfolio) <sub>· updated 4 Oct 2026</sub>
- [New-translator](https://github.com/chillyreward/New-translator) <sub>· updated 29 Jun 2026</sub>
- [gikuyu-translate](https://github.com/chillyreward/gikuyu-translate) <sub>· updated 18 May 2026</sub>
<!--END_SECTION:activity-->

## Across the sand

<!--
  Drawn every day by .github/workflows/sandworm.yml from my contribution
  calendar (private contributions included if enabled on my profile),
  in a sand palette instead of GitHub's green. Lives on the `output` branch.
-->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/chillyreward/chillyreward/output/sandworm-dark.svg">
  <img src="https://raw.githubusercontent.com/chillyreward/chillyreward/output/sandworm-light.svg" width="100%" alt="My GitHub contribution calendar drawn in sand tones, with a sandworm travelling across it.">
</picture>

<br>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/ridge-dark.svg">
  <img src="./assets/ridge-light.svg" width="100%" alt="">
</picture>

<p align="center"><sub><i>Fear is the mind-killer.</i> — Frank Herbert, <i>Dune</i></sub></p>
