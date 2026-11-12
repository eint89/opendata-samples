# OpenData — sample store data

OpenData is a database of verified ecommerce stores. We scan the web ourselves, visit each storefront, and record what we find: the platform it runs on, the technologies and apps installed, the payment gateways it takes, and the business email it publishes — if it publishes one.

The current snapshot (12 November 2026) holds **1,504,744 verified stores**, found across **23,984,359 scanned domains**. "Verified" has a specific meaning here: we fetched the store's own storefront and detected at least one ecommerce technology on it. Every record carries its source URL and the date we last saw it.

## What's in this repo

Four sample files, 25 rows each, pulled in late October 2026 — plus one verification file, `sample-100-unmasked.csv`, covered in "Verify our data yourself" below:

| File | What it shows |
|---|---|
| `samples/opendata-teaser-shopify-2026-10-26.xlsx` | Shopify stores |
| `samples/opendata-teaser-wix-2026-10-26.xlsx` | Wix stores |
| `samples/opendata-teaser-full-2026-10-26.xlsx` | A mix across platforms |
| `samples/opendata-teaser-premium-2026-10-26.xlsx` | The fullest cut: country, apps, payment gateways and a completeness score on top of the basics |

## How the samples are masked

These are teasers, so two things are cut:

- **Domains.** The first 10 rows show the full domain. After that, domains are masked — `dani***.wixsite.com`.
- **Emails.** Where a store publishes a business email, you see the first three letters only — `con***@mocashpub.com`. Most email cells are empty, and that is not a defect in the sample: only 140,579 of the 1,504,744 verified stores publish an email at all. Roughly 1 in 11.

A paid export has none of this. Domains and emails are complete.

## Verify our data yourself

`sample-100-unmasked.csv` (at the top of this repo) breaks the teaser rule on purpose: 100 records from the current snapshot with domains and emails complete — nothing masked. They are published unmasked so anyone can check the stores are live and test the emails themselves before buying anything. Pick any row, visit the store, send the address a test message if you like.

The other samples in this repo stay masked teasers, as described above. The full database is sold per row at https://data.openbio.io.vn.

## Pricing

Everything is sold per row. No subscription, no fixed packages.

- **Full records** (with public business contacts): $4 per 1,000 rows. The rate drops as the pull grows — $3.50 from 10,000 rows, $3.00 from 50,000, $2.50 from 200,000, $2.00 above 500,000.
- **Platform/technology records** (no contacts): $1 per 1,000 rows, and $0.50 above 100,000 rows.
- **Raw domain signals**: $0.20 per 1,000 rows.

Minimum pull is $9.99. Exports come as CSV plus a formatted Excel file. The database is refreshed monthly.

## Check a store free first

Don't take our word for any of this. The store checker at https://data.openbio.io.vn/checker/ looks up any domain in the current snapshot, and a free account gets 30 full-record unlocks a month.

The full database, with filters by platform, country, technology, app and payment gateway, is at https://data.openbio.io.vn — that is where full exports are sold, per row.

## Licence

The samples are free to evaluate, not to redistribute. See `LICENSE.txt`. Questions or removal requests: support@openbio.io.vn
