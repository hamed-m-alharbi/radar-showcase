<p align="center">
  <img src="assets/cover.png" alt="RADAR: every opening, every application, one radar" width="100%">
</p>

<p align="center">
  <b>Radar collects job postings from several sources, scores how well each one fits you, and tracks every application with proof.</b><br>
  Arabic-first · Right-to-left · Dark · Runs on your own machine
</p>

<table>
  <tr>
    <td width="33%" valign="top"><b>Collect</b><br>LinkedIn, company career boards and job-alert emails in one list.</td>
    <td width="33%" valign="top"><b>Score</b><br>A 0–10 fit score for every posting, with the reasons shown.</td>
    <td width="33%" valign="top"><b>Track</b><br>A fixed status flow, and no "submitted" without evidence.</td>
  </tr>
</table>

## The dashboard

<p align="center">
  <img src="assets/dashboard.png" alt="The Radar dashboard: a list of opportunities with fit scores, and the radar on the side" width="92%">
</p>

Every stored posting is a point on the radar. The closer to the centre, the better the fit. A sweep passes over the plate and lights each point in turn. The list beside it is where you search, filter and act.

## Why Radar

Openings are scattered across LinkedIn, company career pages, recruiter emails and regional boards. It is easy to miss a good one, apply twice, or lose track of where an application stands. Radar puts them in one place, shows **how well each fits and why**, and records what happened to every application.

## What it does

### Collects postings from several places

- **LinkedIn public job pages**, searched on demand or at a time you choose each day.
- **Company career boards** that publish open APIs (Greenhouse, Lever, SmartRecruiters, Workable, Ashby).
- **Job-alert emails** from Indeed, Bayt, GulfTalent and others, read from your own inbox.

Radar recognises a posting it has already stored from the same source and does not save it again. The same job published on two different sites can still appear twice.

### Scores the fit, and shows its reasons

Every posting gets a score from 0 to 10, built from three things: how many of your skills it asks for, how close the work is to what you want, and whether it suits your level. Next to the score you see the reasons:

- **matching skills**, the ones you have listed that the posting asks for,
- **skills not in your profile**, the ones it asks for that you have not listed,
- the **years of experience** it requires.

A posting with too little text stays unscored rather than getting a guess, and a score you set yourself is never overwritten.

### Points out gaps, and lets you ask for a second opinion

- **Flags on the card.** When a posting asks for a BI tool such as Power BI, Tableau, Looker or Qlik that is not in your profile, the card says so.
- **Minimum fit filter.** Show only postings scored 5, 7 or 8 and above. Postings not scored yet are left out while a minimum is set.
- **A second opinion, only when you ask.** A button on a scored card asks DeepSeek for its own score and a short reason, shown beside the rule-based one. **Pressing it sends that posting's title and description, and your listed skills, wanted job titles and years of experience, to DeepSeek's API**, after the page asks you to confirm. It is optional and needs an API key. It never changes a score by itself: the rule-based score stays until you choose to adopt the opinion, and an adopted score is then yours and is not overwritten.

### Suggests search preferences from your own words

<p align="center">
  <img src="assets/search-template.png" alt="Search preferences: describe your experience, then pick cities, job titles and skills" width="78%">
</p>

Write a sentence or two about your background and the roles you want, and Radar suggests cities, job titles and skills. **This feature sends the text you type to DeepSeek's API.** It is optional: it only works if you add an API key, and you should not type sensitive personal details. The only other thing that can reach DeepSeek is the second opinion described above, and only when you press its button. You review and edit every suggestion, and nothing is saved until you approve it.

### Follows every application, with evidence

Each opportunity moves through a fixed set of statuses: new, preparing, ready for review, submitted, interview, offer, with skipped, withdrawn and rejected as ways out. Moves that make no sense are not allowed.

<p align="center">
  <img src="assets/record-submission.png" alt="Recording an application together with its evidence" width="78%">
</p>

An application cannot be marked as submitted without proof. You attach a confirmation email, a link, a file path or a short statement, and the date. The record stays with the opportunity, so you can always answer "did I apply, and how do I know?".

### Works the same on a phone

<p align="center">
  <img src="assets/mobile.png" alt="The dashboard on a phone" width="30%">
</p>

The dashboard is built for phone and desktop equally. The radar, the filters and every action are there on a small screen.

## Private by design

- Everything runs on your own computer, and the dashboard is reachable only from that machine.
- Radar never signs in to a job board with your account.
- Your data stays in your own database. The exception is the two optional DeepSeek features above, both started by you: the text you type in the search preferences, and, for one posting at a time, the second opinion.

## Built with

PostgreSQL, FastAPI and n8n, packaged with Docker. The interface is a single static page with no build step.

---

<sub>The screenshots use invented postings and invented employers. Source code is not published here.</sub>
