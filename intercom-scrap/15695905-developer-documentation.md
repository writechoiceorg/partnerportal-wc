PartnerPortal.io is built to connect to the rest of your stack. Whether you want to push leads in, pull data out, or get notified the moment something changes, there's a path that fits how much you want to build.

This page is the starting point. It explains the options at a high level and points you to the right guide for each one.

## What you can do

- **Send leads into PartnerPortal.io** — push leads from your website, marketing automation, or another tool straight into your portal.

- **Pull data out** — fetch leads, account information, and your portal's field schema on demand.

- **Get notified when leads change** — receive a real-time push when a lead is created, updated, or deleted, then sync it into your own system.

- **Automate no-code workflows** — connect PartnerPortal.io to thousands of apps through Zapier without writing any code.

## Three ways to integrate

Pick the path that matches how much engineering effort you want to spend.

- **Zapier**: Connect PartnerPortal.io to other apps (Slack, Google Sheets, your CRM, etc.) through Zapier's visual builder — no code required.

- **REST API**: Standard JSON endpoints to create, read, and update leads, and to discover your portal's field schema. The foundation everything else builds on.

- **Webhooks**: Get a push notification the instant a lead changes, so you don't have to poll. Always used alongside the REST API.

*Many integrations use the REST API and Webhooks together*. Webhooks tell you **when** something happened; the REST API is how you fetch the actual data. Webhooks on their own are a notification mechanism, not a data feed — every webhook still leads to a quick REST call to get the full record.

## Zapier — the no-code option

If you'd rather not write code, start with our official Zapier app. It can:

- *Create a lead in PartnerPortal.io* when something happens in another tool (a form submission, a new spreadsheet row, a CRM record, etc.).

- *Trigger an action elsewhere* when a lead is created or updated in your portal (post to Slack, add a row to Google Sheets, create a deal in your CRM, and so on).

Your portal's custom fields show up automatically as native Zapier inputs, so there's no field-mapping boilerplate.

​**Get started**: [PartnerPortal.io on Zapier](https://zapier.com/apps/partnerportalio/integrations)
​

## REST API — the foundation

The REST API is how you read and write data programmatically. With it you can:

- Create leads (`POST`), update them (`PATCH`), fetch a single lead, or list leads for backfills and reconciliation.

- Discover your portal's lead schema — including any custom fields and picklists you've configured — so your integration always maps the right fields.

It uses OAuth 2.0 access tokens and returns standard JSON. If your plan includes API access, you can generate your own API keys directly in your portal (see below).
​

**Get started**: [Public API Guide](https://gitlab.com/-/snippets/6005790) and [endpoint reference](https://developer.partnerportal.io/docs).

## Webhooks — real-time notifications

Instead of polling the API asking "anything new?", give us a URL and we'll POST to it the moment a relevant event happens. A typical flow:

1. You subscribe to a topic (e.g. `lead/create`) and give us your URL.

2. A lead is created in your portal.

3. We POST a small signed notification — `{ id, topic, timestamp }` — to your URL.

4. Your server verifies the signature, then calls the REST API to fetch the full lead by `id`.

Webhooks cover `lead/create`, `lead/update`, and `lead/delete` today.

**Get started**: [Webhooks Guide](https://gitlab.com/-/snippets/5962251)

## How to get access

How you get credentials depends on your plan:

- **If your plan includes API access**: a portal admin can generate API keys directly in the portal under *Portal Setup → Other → Developer / API Keys*. You can create a key (the secret is shown once — copy it somewhere safe), see your existing keys, and revoke any key at any time. This is the fastest way to get started.

- **If you don't see the Developer / API Keys section**: API access isn't included on your current plan, or you don't have admin permissions. You can upgrade from your portal or contact support.

Either way, you'll end up with:

- A **Client ID** and **Client Secret** (your credentials)

- An **Audience** (a URL that identifies our API)

- Your **Company ID** (identifies your portal in API requests)

**Treat your Client Secret like a password.** Don't paste it into email, Slack, or ticketing systems. If a key is ever exposed, revoke it from the Developer / API Keys page (or contact us) and create a new one.
​

The same credentials work for both the REST API and Webhooks.
​

## Need help?

For anything that doesn't behave as expected — auth errors, unexpected responses, or design questions like "should I use webhooks or polling for this?" — contact our support team. Tell us what you're trying to build and we'll point you at the right approach. Creating a test partner allows you to see the registration process, portal access, and partner experience firsthand.