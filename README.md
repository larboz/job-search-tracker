# Job Search Tracker

A live, editable dashboard for tracking job applications — built with Claude.

**Live tracker:** https://claude.ai/artifact/1MDwghr75USs7xfhSSb1Tg

## What it does

- Tracks every application: company, role, date applied, status (Pending / Interviewing / Offer / Rejected / Withdrawn), and rejection date when applicable
- Statuses and dates are editable directly in the page — changes sync live for anyone with access
- A scheduled scan runs 4x/day against Gmail to add newly discovered applications and catch explicit rejection emails, without ever overwriting a manually-set status (Interviewing/Offer/Withdrawn stay under manual control)
- Stat tiles and charts (rejection rate, time-to-rejection, weekly volume) recompute live from the underlying data

## Files

- `dashboard.html` — the full source of the tracker page (charts, editable table, add/delete, live sync logic)
- `index.html` — redirects here on GitHub Pages to the live, data-backed version, since the live sync only runs on its hosted Claude artifact page

## Stack

Single-file HTML/CSS/JS. Live sync and the shared database run through Claude's Artifact platform capabilities — this repo is a source/portfolio copy, not a standalone deployable app.
