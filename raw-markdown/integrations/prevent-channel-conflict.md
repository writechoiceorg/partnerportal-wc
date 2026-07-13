---
title: "Can you prevent Channel Conflict?"
description: "Yes we can; we cache your connected CRM's deals (or custom object configuration) for a quick search prior to approving any lead."
---

When pushing any lead from PartnerPortal.io to your CRM, we've designed a lead approval system that will prevent duplicates from being created.

Below, we've included a quick example of our type-ahead feature. In the clip, you'll notice new leads can be 'linked' to an existing deal in HubSpot. This will work similarly for other CRMs, though the behavior may differ slightly. This is the first step to preventing partners from registering duplicate leads.

When approving a lead, you'll have the option to link to an existing deal in your CRM or create a new deal (again, behavior will vary slightly depending on which CRM integration you are using).

## HubSpot CRM (automatic de-dupe):

- Our first step will be to find an existing company using the domain name of the company. It uses it if it is found, otherwise, it creates one.

- Using the email, we'll search for an existing contact. It uses it if found, otherwise, it creates one.

- The contact is associated with the company.

- A new deal is created from your PartnerPortal.io data.

- The contact and company are associated with this new deal. No de-dupe is involved on the deal stage of this creation pipeline.

## Salesforce CRM (de-dupe):

- De-duplication settings are determined by your Salesforce configuration. Salesforce does not give us any insight into your specific configuration. We will detect if Salesforce creation fails due to de-dupe and surface that error to you.

## Chan·nel /ˈCHanl/ + Con·flict (official definition)

Due to the variety of distribution channels businesses have, there can be several types of channel conflicts. Channel conflict occurs when a brand's lack of communication or transparency hinders its partners' sales. **Not anymore!**
