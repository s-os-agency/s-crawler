# Crawler — plain-language README

## What this is
A website crawler: give it a starting web page and it visits that page, follows the links to a depth you choose, and lists every page it found. It also keeps a clear record of how it reached each page.

## Who it's for
Anyone who needs to map out a website: what pages exist, how they link together and which ones are broken.

## What it does today
- Starts from one or more web addresses. The start page is "level 0"; pages it links to are level 1, and so on, up to level 10.
- Can stay on the same website only, if you want.
- Loads pages in a real browser engine (Playwright), so pages built with JavaScript work.
- Cleans up addresses and skips pages it has already seen.
- For each page it records:
  - the address
  - the level
  - the title
  - the response code (e.g. 200 = OK)
  - which page linked to it
  - its links
  - any error
- Offers a small web service you can call:
  - `POST /crawl` starts a crawl
  - `GET /health` checks it's running
- Has a live web page: https://s-crawler-live-5k218z.v2.appdeploy.ai/ . That page uses a separate hosted crawler, not the Python one in this repo.
- Has automated tests and runs checks on GitHub.
- Publishes a description of itself that AI tools can read (`llms.txt` and similar).
- A private ChatGPT plugin exists for using it from ChatGPT.

## How to run it
You need Python.
```bash
pip install -r requirements.txt
playwright install chromium
python app.py
```
Then, in another window:
```bash
curl -X POST http://localhost:8080/crawl \
  -H 'Content-Type: application/json' \
  -d '{"url":"https://example.com","max_depth":5,"same_domain":true}'
```

## Current status and known gaps
Not done yet:
- exporting results to files
- pausing and resuming a long crawl
- detecting when a page's content has changed

Only crawl sites you are allowed to crawl.

## Where things live
| File / folder | What's in it |
|---|---|
| `app.py` | The crawler and its web service |
| `requirements.txt` | Python packages it needs |
| `tests/` | Automated checks (folder name not yet confirmed) |
| `.github/` | GitHub automatic checks |
