<p align="center">
  <img src="assets/cover.png" alt="RADAR: every opening, every application, one radar" width="100%">
</p>

<p align="center">
  <b>A private job-search pipeline that finds postings, scores how well they fit you, and follows every application to the end.</b>
</p>

<p align="center">
  Arabic-first · Right-to-left · Dark · Runs on your own machine
</p>

---

## Why Radar

Job hunting is scattered. Openings appear on LinkedIn, on company career pages, in recruiter emails and on regional boards, and the same posting shows up in three places. It is easy to miss a good one, apply twice, or lose track of where an application stands.

Radar brings all of it into one dashboard, keeps a single copy of each posting, tells you **how well it fits and why**, and records what happened to every application.

## The dashboard

<p align="center">
  <img src="assets/dashboard.png" alt="The Radar dashboard: a list of opportunities with fit scores, and the radar on the side" width="92%">
</p>

Every stored posting is a point on the radar. Closer to the centre means a better fit. A sweep passes over the plate and lights each point in turn, so the whole pipeline can be read at a glance. The list beside it is where you search, filter and act.

## What it does

### Finds postings from many places

- **LinkedIn public job pages**, searched on demand or at a time you choose each day.
- **Company career boards** that publish open APIs (Greenhouse, Lever, SmartRecruiters, Workable, Ashby).
- **Job-alert emails** from Indeed, Bayt, GulfTalent and others, read from your own inbox.

Each posting is stored once, however many sources it came from.

### Scores the fit, and shows its reasons

Every posting gets a score from 0 to 10, built from three things: how many of your skills it asks for, how close the work is to what you want, and whether it suits your level. Next to the score you see the reasons:

- the skills you **have** that it asks for,
- the skills you **lack**,
- the years of experience it requires.

Nothing is a black box, and a score you set yourself is never overwritten.

### Lets you describe your experience in plain words

<p align="center">
  <img src="assets/search-template.png" alt="Search preferences: describe your experience, then pick cities, job titles and skills" width="78%">
</p>

Write a sentence or two about your background and the roles you want. A language model suggests the cities, job titles and skills for your search preferences. You review and edit them before anything is saved. Only the text you type is sent, and nothing is stored until you approve it.

### Follows every application, with evidence

Each opportunity moves through a fixed set of statuses: new, preparing, ready for review, submitted, interview, offer, with skipped, withdrawn and rejected as ways out. Moves that make no sense are not allowed.

<p align="center">
  <img src="assets/record-submission.png" alt="Recording an application together with its evidence" width="78%">
</p>

An application cannot be marked as submitted without proof. You attach a confirmation email, a link, a screenshot path or a note, and the date. The record stays attached to the opportunity, so you can always answer "did I apply, and how do I know?".

### Works the same on a phone

<p align="center">
  <img src="assets/mobile.png" alt="The dashboard on a phone" width="30%">
</p>

The dashboard is built for phone and desktop equally. The radar, the filters and every action are there on a small screen.

## Private by design

- Everything runs on your own computer. The dashboard is reachable only from that machine.
- No account on any job board is ever used or touched.
- Your data stays in your own database.

## Built with

PostgreSQL, FastAPI and n8n, packaged with Docker. The interface is a single static page with no build step.

---

<sub>The screenshots use invented postings and invented employers. Source code is not published here.</sub>
