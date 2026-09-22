# CarrierLookup resources

Official technical resources, guides and developer articles for **CarrierLookup** — original carrier, line type and allocation lookups.

- **Website:** https://carrierlookup.online
- **Blog:** https://carrierlookup.online/blog
- **API documentation:** https://carrierlookup.online/api-docs
- **Pricing:** https://carrierlookup.online/pricing

## What is in this repository

This repository is the public home for CarrierLookup technical writing that is published outside the website:

- **[Issues](../../issues)** — short technical notes on integration, result interpretation and operational practice.
- **[Discussions](../../discussions)** — longer announcements and product guidance under the *Announcements* category.

The canonical version of every product fact lives on the website. Where an article and the site disagree, the site wins.

## Official API example repositories

One repository per product, each with an OpenAPI contract, a machine-readable `product.json`, an `llms.txt` summary and runnable examples in seven languages.

| Product | Shape | Repository |
|---|---|---|
| [Original Carrier Lookup](https://github.com/carrierlookup/phone-carrier-lookup-api) | Realtime | `phone-carrier-lookup-api` |
| [Bulk Global Carrier Lookup](https://github.com/carrierlookup/bulk-carrier-lookup-api) | Bulk (async) | `bulk-carrier-lookup-api` |

A **realtime** check answers inside the same HTTP response (`POST /api/v1/check`, or `POST /api/v1/batch-check` for up to 100 identifiers). A **bulk task** takes a file and answers later (`POST /api/v1/bulk-tasks`). They are separate endpoints and are not interchangeable.

## Responsible use

CarrierLookup results are **point-in-time signals**. A result describes what a provider reported at the moment of the check — it is not identity verification, not proof of ownership, and not permission to contact anyone. Use the API only for identifiers you are authorized to process, and comply with applicable privacy laws and platform terms.

Third-party trademarks belong to their respective owners; no affiliation or endorsement is implied.

---

*Maintained by CarrierLookup. Questions and integration problems: https://carrierlookup.online/contact*
