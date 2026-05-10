 Privacy Policy for Planner (Basic Planner)

**Last Updated: May 10, 2026**

## Introduction

This Privacy Policy describes how **Planner** (“Basic Planner”, “we”, “our”, or “the app”) handles information when you use our mobile application. We aim to be transparent and to align with common expectations for privacy on Google Play and under laws such as the GDPR (including Norway) and, where applicable, the CCPA.

**This policy is provided for your convenience and does not constitute legal advice.** If you need legal advice, consult a qualified professional.

---

## Developer Information

| | |
|---|---|
| **App name** | Planner (listed as Basic Planner where the full name is shown) |
| **Developer** | Basic Organizer |
| **Contact email** | basicorganizer.post@gmail.com |

This app is developed and maintained as an independent project. Support response times may vary.

---

## Summary (quick read)

- Your **calendar content** (events, tasks, notes, special dates you enter) is stored **on your device** (SQLite + app preferences), not on our servers.
- The app **does not** include advertising SDKs or analytics SDKs in the current version.
- **Optional internet use:** if you choose a **country for public holidays** in Settings, the app may download **public holiday lists** for that country/year from a third-party API. Your personal entries are **not** uploaded with that request.
- **Report a bug** opens your email app; anything you send is between you and your email provider.
- **Get organized / More apps** opens the Google Play Store (Google’s policies apply there).

---

## Information We Collect and Store

### Data stored locally on your device

All primary user content stays **on your device**, in app-private storage:

**SQLite database (`PlannerDB`):**

- **Events:** titles, notes, dates, start/end times, recurrence settings, colour choice, and related fields needed to show your calendar.
- **To-dos / tasks:** titles, dates, scope (day/week/month/year), completion status, optional move-to-next behaviour, sort order, and related fields.

**Shared preferences (app settings), including:**

- Display preferences (e.g. date format, time format, first day of week, completed-task behaviour).
- **Country for public holidays** (ISO country code used only to request public holiday data—see below).
- **Special dates / occasions** you add (e.g. birthdays and similar entries stored as structured data in preferences).

We **do not** operate our own backend that receives this content in the normal operation of the app.

### Data transmitted over the internet (limited)

**Public holidays (optional)**

- If you select a **country for public holidays** in Settings, the app may request data from **Nager.Date** (`date.nager.at`), a public API that returns **public holiday dates and names** for the selected **calendar year** and **country code**.
- The request needs **only** the year and country—not your events, tasks, notes, or account information.
- Holiday results may be **cached in memory** on your device to reduce repeat requests.
- If you choose **no country**, this fetch is not used for that purpose.

**Other links that leave the app**

- **Report a bug:** Opens your installed email app with a `mailto:` link to **basicorganizer.post@gmail.com**. Any message, attachments, or metadata are handled by **your email provider** and your chosen email app—we only receive what you choose to send.
- **More apps / Play Store:** Opens Google Play (app or browser). **Google’s** privacy policy and terms apply to that experience.

We do **not** sell your personal information.

---

## Data we do not collect (in the app as built)

The current app version does **not**:

- Send your events, tasks, or notes to our servers (we do not host such a service for this app).
- Use in-app **advertising** or **analytics** SDKs as part of the distributed build described here.
- Request **precise location** or **contacts**.
- Access **photos** or **files** outside what the system provides for normal app storage.

---

## How we use information

- Local data is used **only** to provide planner features (calendar views, reminders of what you entered, settings you chose).
- Optional holiday data is used **only** to show public holidays for the country/year you selected.

---

## Legal bases (EEA / Norway – GDPR)

Where the GDPR applies, we rely primarily on:

- **Performance of the service / legitimate interests** in running a local planner and optional non-sensitive holiday lookup you trigger by settings.

You may **withdraw consent** for optional behaviour where consent applies by disabling the related setting (e.g. clearing the holidays country) or uninstalling the app.

---

## Retention and deletion

- You can **delete or edit** events, tasks, and special-date entries within the app subject to the features provided.
- **Uninstalling** the app removes locally stored app data from your device under normal Android behaviour (subject to your device manufacturer and backup settings).
- **Automatic cloud backup** is disabled for this app in its manifest (`allowBackup` is `false`), which avoids Android’s default backup of app data to Google’s backup infrastructure for this app—**device policies and manufacturer behaviour may still vary**.

---

## Security

- Data stays in **app-private storage** on the device; other apps cannot read it without system-level access or a compromised device.
- Security also depends on **your device** (screen lock, OS updates, malware avoidance).

No method of storage or transmission is 100% secure.

---

## Children’s privacy

The app is a general-purpose planner. We do not knowingly market it solely to children or seek personal information from children. If you believe a child has provided information to us by email, contact us and we will address it reasonably.

---

## International users & rights

Depending on where you live, you may have rights to **access**, **rectify**, **erase**, **restrict processing**, **object**, or **data portability**, and to **lodge a complaint** with a supervisory authority.

Because most data is **local to your device**, you can often exercise control directly in the app or by uninstalling. For privacy requests sent by email, we will respond within reasonable timelines; **EEA users** may receive a reply within **30 days** where the GDPR requires it, with possible extension for complex requests.

---

## Third-party services you should read about

- **Nager.Date** – public holiday API provider; see their terms and privacy policy if you use holiday lookup.
- **Google Play / Google** – when you open Play from the app or install updates.
- **Your email provider** – when you send a bug report.

---

## Changes to this policy

We may update this policy from time to time. The **Last Updated** date will change. Significant changes may be noted in the Play Store listing or app description where practical.

---

## Contact

**Email:** basicorganizer.post@gmail.com  
**Developer:** Basic Organizer

When contacting us, please describe your request clearly. If you are in the EEA/Norway and invoke GDPR rights, mention that so we can route your request appropriately.

---

## Disclaimer

The app is provided **“as is”**. We strive to describe data practices accurately but cannot guarantee that every future device or OS behaviour is captured here. This policy is not a contract.

---

## Consent

By using Planner (Basic Planner), you acknowledge this Privacy Policy. If you do not agree, please do not use the app.
