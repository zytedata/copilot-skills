# Changelog

## 0.2.3 (2026-07-16)

### Improved

- `/scrape-scrapy-cloud`: if a Scrapy Cloud job was started the skill now waits
  for it to finish and reports the results. If the results look wrong (errors,
  wrong items, low coverage) it tries to fix the problems and rerun the job.
- `/scrape`, `/scrape-spec` and other related skills: if all required fields
  can be extracted from list pages, the skills will generate code that does
  that and doesn't request detail pages.
- `scrape-zyte-login`: the login flow now uses OAuth and stores credentials in
  the project's `.env` file for reuse by the scraping skills.

### Fixed

- `/scrape-review-schema`: fixed problems when running the review on Windows.

## 0.2.2 (2026-07-03)

Initial release.
