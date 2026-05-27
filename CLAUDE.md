# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a **Mintlify documentation project** for [PartnerPortal.io](https://partnerportal.io), a SaaS partner portal management platform. It contains 66 MDX help articles served as a Mintlify docs site.

## Commands

```bash
# Install CLI (requires Node >= 20.17.0)
npm install -g mintlify

# Preview locally with live reload
mintlify dev

# Validate config and pages before deploying
mintlify validate
```

## Key Files

- `docs.json` — Mintlify configuration: theme, colors, and full navigation tree (tabs → groups → pages)
- `index.mdx` — Landing page for the docs site

## Repository Structure

Documentation is organized into 5 top-level categories:

- `get-started/` — Onboarding: sign-up, pricing, team setup, partner program configuration
- `portal-setup/` — Portal config: SSO, billing, dashboard branding, team roles/permissions
- `partner-and-leads/` — Partner management, lead lifecycle, partner user management
- `integrations/` — CRM (HubSpot, Salesforce, Pipedrive, Zoho), payments (PayPal), accounting (QuickBooks), Slack, Zapier
- `features/` — Payments/commissions, resource center, opportunities, metrics, multi-language

## Platform Context

Key concepts that appear across many articles:

- **Partner statuses**: pending → approved → active; can be suspended or declined
- **Partner groups**: used for access control on resources, lead routing, and permissions
- **Lead phases**: customizable pipeline stages for lead lifecycle management
- **CRM sync**: bidirectional field mapping between PartnerPortal leads and CRM deals/contacts; HubSpot pipeline mapping is the most complex integration
- **Payments**: commission structures support percentage, fixed, and recurring models; PayPal is used for partner payouts
- **SSO**: powered by Auth0, supports Okta, Google Workspace, Azure AD, and LDAP
- **Resource Center**: document sharing with partner group–based access control

## Documentation Conventions

- **File naming**: lowercase hyphenated (e.g., `how-to-connect-hubspot.md`)
- **Format**: Step-by-step guides with numbered steps; screenshots embedded via Intercom media URLs
- **Cross-references**: Articles link to related docs by relative path or full URL
- **Contact info used in articles**: sales@partnerportal.io, support@partnerportal.io, getanswers@partnerportal.io
- **Pricing tiers referenced**: Free (2 partners, 5 leads), Growth $249/mo (50 partners, 300 leads), Enterprise $499/mo (unlimited)
