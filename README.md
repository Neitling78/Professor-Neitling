# Professor Neitling: Microbiology

Public faculty page for Professor Cassandra Neitling (Microbiology, Folsom Lake College).
Personal page, not an official Folsom Lake College website.

**Live:** https://neitling78.github.io/Professor-Neitling/
**Preview with placeholders visible:** add `?draft=1` to the URL.

## Tabs
1. About Microbiology
2. Class Schedule
3. Assignments & Grading
4. Recommendation Letters (student request form)
5. Career Opportunities

## How it works
- `index.html` is the entire site: one self-contained file with no build step, served by GitHub Pages.
- The letter request form posts to a Google Apps Script web app running on Casie's Google account (set `FORM_ENDPOINT` in `index.html`).
  That script stores the request in a Google Sheet, emails Casie, and drafts letters through the Anthropic API.
  The API key lives only in Apps Script's Script Properties, never in this repo.
- Until `FORM_ENDPOINT` is set, the public form shows "requests will open soon."

## Privacy rules for this repo
- No student data, API keys, or class meeting times/rooms are ever committed here.
- This repo is public.

## Update the site
Edit `index.html`, then from this folder:

    git add -A && git commit -m "describe the change" && git push

GitHub Pages republishes in about a minute.
