---
title: SyncSpot Privacy Policy
---

# SyncSpot — Privacy Policy

_Last updated: July 15, 2026_

SyncSpot ("the extension") is a Chrome browser extension that lets you create and update
contacts in your own HubSpot CRM from a LinkedIn profile or conversation you are viewing.
This policy explains what data the extension handles and where it goes.

**The short version: your CRM data moves in exactly one direction — from the page you are
looking at, in your browser, to your own HubSpot account — and only when you ask it to. We
never see, collect, store, or sell any of it. The only thing the extension sends to us is
optional usage statistics (event names, your display name and your own profile link — never
page content, messages, contacts or your token), and you can turn that off in Settings.**

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
- **Usage statistics** (optional, on by default): event names, a timestamp, the extension
  version, a random installation identifier, your display name and the URL of your own
  LinkedIn profile — detailed in the "Usage statistics" section below.

## Where data is stored

All settings and caches are stored **locally in your browser** using Chrome's extension
storage (`chrome.storage.local`). The extension has no backend of its own; the only data
we hold outside your browser is the optional usage statistics stored with our processor
(PostHog, EU) — see the "Usage statistics" section below.

## Where data is sent

Your CRM data goes to exactly one place: **the HubSpot API (`api.hubapi.com`)**, over HTTPS,
authenticated with your own token, into your own HubSpot account. If usage statistics are
enabled (see below), small usage events additionally go to our analytics provider (PostHog,
EU-hosted). Beyond the LinkedIn page you are already on, the extension talks to no host
other than the HubSpot API and (if enabled) PostHog. LinkedIn pages are only read, never
written to, and no data is sent to LinkedIn.

## What we do NOT do

- We do not operate any servers; your CRM data never passes through us. The only thing
  we receive is the optional usage statistics described below.
- We do not collect anything beyond the usage statistics described below — no page content,
  no browsing history, no crash dumps — and you can turn even that off.
- We do not sell data. We do not transfer it to any third party except the optional
  usage statistics sent to our analytics provider (PostHog, our processor) described below.
- We do not use data for advertising or for creditworthiness/lending decisions. Usage
  statistics are used solely to see that the tool works and how the team uses it (our
  legitimate interest as an internal team tool); events carry the operator's name so the
  team can see adoption, and you can opt out at any time.
- We do not perform bulk or background collection: the extension only reads the page you
  have open, and writes to HubSpot only on your explicit action (except auto-sync, which
  you must turn on yourself and can turn off at any time).

## Your controls

- Usage statistics can be turned off at any time (Settings → Usage stats).
- Auto-sync of conversations is **opt-in** (Settings → Auto-sync) and can be disabled at
  any time.
- Removing your token from the settings page immediately cuts the extension off from your
  HubSpot account; you can also revoke the Private App token on the HubSpot side.
- Uninstalling the extension deletes all locally stored settings and caches. Usage
  statistics already sent are deleted on request — see "Usage statistics" below.
- Data written into HubSpot (contacts, notes, logged conversations) lives in your HubSpot
  account under your control; delete it there like any other CRM record.

## Data subjects' rights (GDPR/CCPA note)

LinkedIn profile information is personal data of the people whose profiles you view. You
(and your organization) act as the data controller for whatever you choose to save into
your CRM; SyncSpot is a local tool and does not itself retain that data. Please make sure
your use of the extension complies with the privacy laws that apply to you.

## Usage statistics (optional)

SyncSpot sends usage statistics to our analytics provider (PostHog, hosted in the EU):
event names (e.g. "sync", "contact_created"), for some events a coarse mode flag (e.g.
whether a sync was manual or automatic), a timestamp, the extension version, a random
installation identifier, a display name and the URL of your own LinkedIn profile. The name
and URL identify **you, the operator** — the name is the one you enter in Settings or, if
left blank, the name derived from your OWN profile (read once from your feed); they are
never the name or data of anyone whose profile you view.

The same channel carries diagnostic events (e.g. "dom_selector_miss", "hubspot_api_error")
so we learn about breakages early; on top of the standard fields above, these add only
coarse technical attributes of the failure — e.g. which category of API endpoint failed
and its HTTP status code, or which part of the page layout was not recognized — never
record identifiers, free-text error messages or page content.

Usage statistics never include message contents, LinkedIn profile data of people you view,
HubSpot contact data or your token. Sharing is on by default and you can turn it off at any
time in Settings → Usage stats.

Usage statistics already sent (including your name and profile link) are stored with our
processor PostHog (EU) and are not deleted by uninstalling the extension. We keep them
only while the tool is in active use by the team; email **mykhailo.pihosh@gmail.com** and
we will delete your events and person profile. As with any web request, our provider
technically receives your IP address when an event is sent; we have disabled geolocation
enrichment and do not use IP addresses.

## Changes to this policy

If the extension's data handling ever changes (for example, a future version adds new
kinds of telemetry or a backend service), this policy will be updated and the "Last
updated" date changed before the new version ships.

## Contact

Questions or concerns: **mykhailo.pihosh@gmail.com**

