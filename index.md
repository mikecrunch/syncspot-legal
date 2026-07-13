---
title: SyncSpot Privacy Policy
---

# SyncSpot — Privacy Policy

_Last updated: July 9, 2026_

SyncSpot ("the extension") is a Chrome browser extension that lets you create and update
contacts in your own HubSpot CRM from a LinkedIn profile or conversation you are viewing.
This policy explains what data the extension handles and where it goes.

**The short version: SyncSpot has no servers. Your data moves in exactly one direction —
from the page you are looking at, in your browser, to your own HubSpot account — and only
when you ask it to. We never see, collect, store, or sell any of it.**

## Who we are

SyncSpot is developed and maintained by an independent developer.
Contact: **mykhailo.pihosh@gmail.com**

## What the extension does

When you open a LinkedIn profile, SyncSpot reads the information already visible to you on
that page (name, headline, job title, company, location, profile URL, profile photo) and
shows it in a side panel. When you click "Add to HubSpot" or "Sync", that information is
sent directly from your browser to the HubSpot API (`api.hubapi.com`) using the HubSpot
Private App token **you** created and pasted into the extension's settings.

If you use the message features (manual "Sync to HubSpot" button in a conversation, or the
optional auto-sync setting, which is **off by default**), the text of the currently opened
LinkedIn conversation is sent to your HubSpot account as a logged communication on the
matched contact.

## Data the extension processes

- **LinkedIn page content you can already see**: name, headline, job title, company,
  location, profile URL, profile photo, and — only if you use the message features —
  the messages in the conversation you have open.
- **Your HubSpot data**: contact records the extension reads and writes on your behalf
  (fields such as email, phone, job title, company, owner, lifecycle stage, notes,
  logged communications).
- **Your settings**: your HubSpot Private App token, property-mapping choices, message
  templates, the auto-sync on/off flag, and a small technical cache that maps LinkedIn
  profile identifiers to profile URLs (used to match conversations to contacts).

## Where data is stored

All settings and caches are stored **locally in your browser** using Chrome's extension
storage (`chrome.storage.local`). Nothing is stored anywhere else. The extension has no
backend, no database, and no analytics or telemetry of any kind.

## Where data is sent

To exactly one place: **the HubSpot API (`api.hubapi.com`)**, over HTTPS, authenticated
with your own token, into your own HubSpot account. The extension makes no other network
requests. LinkedIn pages are only read, never written to, and no data is sent to LinkedIn.

## What we do NOT do

- We do not operate any servers and cannot see your data.
- We do not collect analytics, telemetry, crash reports, or usage statistics.
- We do not sell or transfer data to any third party.
- We do not use data for advertising, profiling, or creditworthiness purposes.
- We do not perform bulk or background collection: the extension only reads the page you
  have open, and writes to HubSpot only on your explicit action (except auto-sync, which
  you must turn on yourself and can turn off at any time).

## Your controls

- Auto-sync of conversations is **opt-in** (Settings → Auto-sync) and can be disabled at
  any time.
- Removing your token from the settings page immediately cuts the extension off from your
  HubSpot account; you can also revoke the Private App token on the HubSpot side.
- Uninstalling the extension deletes all locally stored settings and caches.
- Data written into HubSpot (contacts, notes, logged conversations) lives in your HubSpot
  account under your control; delete it there like any other CRM record.

## Data subjects' rights (GDPR/CCPA note)

LinkedIn profile information is personal data of the people whose profiles you view. You
(and your organization) act as the data controller for whatever you choose to save into
your CRM; SyncSpot is a local tool and does not itself retain that data. Please make sure
your use of the extension complies with the privacy laws that apply to you.

## Changes to this policy

If the extension's data handling ever changes (for example, a future version adds optional
telemetry), this policy will be updated and the "Last updated" date changed before the new
version ships.

## Contact

Questions or concerns: **mykhailo.pihosh@gmail.com**

## Usage statistics (optional)

SyncSpot can send anonymous usage statistics to our analytics provider (PostHog, EU-hosted):
event names (e.g. "sync", "contact_created"), a timestamp, the extension version, a random
installation identifier, and a display name. The display name is either the one you enter in
Settings or, if left blank, your OWN LinkedIn name (derived from your own profile URL read once
from your feed) — never the name of anyone whose profile you view.
It never includes message contents, LinkedIn profile data, HubSpot contact data or your token.
You can turn this off at any time in Settings → Usage stats.
