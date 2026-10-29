# pdi-news

Daily freight and trucking news for pdi-industries.com.

The site's news page (https://pdi-industries.com/news) reads news.json from this repository. Three stories go up each day, at 9 AM, 12 PM and 3 PM Central, each with the sources it was written from.

## Uptime alerts

`.github/workflows/uptime.yml` checks https://pdi-industries.com/ and https://pdi-industries.com/api/healthz every 10 minutes. After two failed checks in a row it opens an issue titled "pdi-industries.com is down" (or comments on the open one), and GitHub emails the repo owner. It closes the issue when the site answers again. It uses only the built-in `GITHUB_TOKEN`; there are no secrets in this repo.
