# Privacy Policy for Basic Planner

**Last Updated: August 30, 2026**

## Introduction

This Privacy Policy explains how Basic Planner ("we", "our", or "the app") collects, uses, and handles information in connection with the Android mobile application (package name: `com.basicorganizer.planner`).

This policy covers the Basic Planner Android application published by Basic Organizer. It does not govern Google Play, email providers, Google’s backup systems, the Nager.Date public-holidays service, device manufacturers, or other third-party services. Those parties have their own policies.

Basic Organizer develops and maintains the app as an independent project. The application does not operate developer-run servers and does not transmit planner content to Basic Organizer or to any server operated by Basic Organizer. This document is provided for transparency and does not constitute legal advice.

## Developer Information

**App Name:** Basic Planner (device label: Planner)  
**Developer:** Basic Organizer  
**Contact Email:** basicorganizer.post@gmail.com  
**Distribution:** Google Play Store

**Note:** This app is developed and maintained as an independent project. While we strive to provide reliable service and support, response times and feature development may vary based on available resources.

## Information We Collect

### Data Stored Locally

Application data required for ordinary operation is stored **locally on the device**:

- **Events:** Titles, notes, dates, start and end times, recurrence settings (including excluded dates and end dates), color indices, and creation timestamps
- **To-dos, tasks, and goals:** Titles, dates, scope (day / week / month / year), completion status, importance, sort order, “move to next month” settings, and optional day-reminder settings (whether a reminder is on and at what time)
- **Day colors:** Color marks applied to specific dates
- **Special dates:** Annual entries (for example birthdays and anniversaries) and one-time dates for the current year, including optional reminder settings (on the day, days before, and reminder time)
- **App preferences:** Language (including system default); date and time display format; 24-hour vs 12-hour time; first day of the week; default calendar view; light or dark theme; behavior when a task is completed; public-holidays country selection; per-month color label meanings; and backup choices (including the backup folder selected, if any)

This information is stored in a local SQLite database and in app-private SharedPreferences. The app does **not** transmit it to Basic Organizer or to any server operated by Basic Organizer. Optional backup features can create copies of this data outside the device, as described in the backup section below.

Event titles, notes, special-date names, to-do titles, and other text entered by the user may constitute personal or sensitive information depending on content. Users are responsible for the information they choose to enter into the app, including determining whether such information is appropriate to store on their device or in any backup location. Users should not use the app to store information that they are legally prohibited from storing, information belonging to another person without appropriate authorization, passwords, authentication credentials, financial credentials, or other information requiring a level of security that the app does not provide. The developer does not use user-entered content for advertising or analytics.

### Public holidays (optional network use)

If a country is chosen in Settings for public holidays, or if the app uses a supported default country based on the device locale (when the user has not chosen “none”), the app downloads public holiday data for that country from the independent [Nager.Date](https://date.nager.at) API (`https://date.nager.at/api/v3/PublicHolidays/{year}/{countryCode}`).

- The request contains the selected country code and year in the request URL. It also sends a generic app User-Agent string (`BasicOrganizer-Planner/1.0 (Android)`). **No events, to-dos, notes, special dates, or other planner content is included.** As with ordinary internet communications, the request may also be accompanied by technical network information, such as an IP address, that may be visible to the service or its infrastructure. Basic Organizer does not receive this information through the app and does not control how Nager.Date or its infrastructure logs, retains, or otherwise processes such information.
- Successful responses are cached on the device in app-private storage so the app can show holidays when offline. That cache is **not** included in the app’s Google Backup or folder backup files described below.
- If no country applies (for example the user chose “none” in Settings, or the device locale does not match a supported country), **no holiday API requests are made.**
- Nager.Date is operated independently of Basic Organizer. Basic Organizer does not control Nager.Date's availability, security, logging, retention, or handling of network requests. Any processing of the request by Nager.Date is governed by Nager.Date's own terms and policies.

This is the **only** purpose for which the app uses the Android **INTERNET** permission in its own code. That permission is not used to transmit planner content to Basic Organizer or to any server operated by Basic Organizer.

### Reminders and notifications (optional)

Reminders are **optional** and are configured per special date or per day to-do when the user turns them on.

- **Special dates:** Optional notification on the day and/or a configurable number of days before, at a time chosen by the user.
- **Day to-dos:** Optional notification on the due day at a time chosen by the user (including for to-dos set to move forward until completed).
- **Calendar events** do not currently offer reminders in the app.

When enabled, reminders are scheduled **locally on the device** using Android’s alarm and notification system. Reminder text is derived from titles the user entered (for example a birthday name or to-do title). **Reminder content is not transmitted to Basic Organizer or to any server operated by Basic Organizer.**

On Android 13 and later, the app may request the **POST_NOTIFICATIONS** permission (typically when the app is opened) so that reminder notifications can be shown if the user has enabled reminders. If that permission is denied, or if notifications are blocked in system settings, reminders may not appear on screen even though reminder settings remain stored locally.

After a device restart, the app reschedules enabled reminders locally. Reminder delivery can be affected by Do Not Disturb, battery optimization, exact-alarm restrictions, manufacturer-specific power management, or other system settings outside the developer’s control. **Reminders are not guaranteed to fire at the exact intended moment.**

Tapping a reminder notification opens the app. No third-party analytics or advertising SDK receives notification events through the app.

### Optional backups

Backup is **optional**. In the app, both Google Backup and folder backup are **off by default** until switched on in **Backup & Restore**. Either option, both, or neither may be used.

**Google Backup**

- The app allows Android backup (`allowBackup`), but planner data is included in a backup that uses the Android backup system only when the in-app Google Backup option is enabled. A custom backup agent includes the planner database and related preference files only when that option is switched on; if it is off, the agent backs up nothing.
- Planner data is added to Google Backup only when the Google Backup option is switched on in **Backup & Restore** *and* Google Backup is enabled in device settings. When included, that backup contains:
  - The planner SQLite database (events, to-dos, day colors, and related fields including reminder flags and times stored there)
  - Planner settings (including special dates, color label meanings, language, theme, default view, holidays country, date/time formats, and similar preferences)
  - Backup preference settings (such as opt-in flags and, if folder backup was configured, the chosen folder location)
- That backup is handled by Google under [Google’s Privacy Policy](https://policies.google.com/privacy), not by the Basic Planner developer. **The developer does not receive, access, or host that data.**
- The option may be turned off in the app at any time. Turning it off stops the app from adding planner data to later backups that use the Android backup system. Copies already stored by Google remain until deleted in Google account or device backup settings.
- The app’s backup configuration applies to backup mechanisms that use the Android backup system. Device manufacturers may provide separate transfer or migration tools whose behavior can vary by device and Android version and which may be governed by the manufacturer’s own settings and policies.
- The developer does not control third-party device backup, migration, cloning, synchronization, restoration, or transfer mechanisms. Such mechanisms may copy, retain, modify, omit, or otherwise process application data independently of the app’s own backup settings. Their operation is governed by the applicable device manufacturer, operating system, or service provider.

**Folder backup**

- Only when switched on and a folder is chosen with the system file picker (for example a folder on the device, or in the user’s own cloud storage).
- When folder backup is enabled, a backup file is written promptly, then about once a day (the schedule may be delayed if the battery is low). The app attempts to keep the **5 most recent** backup files it created in that folder and may delete older backup files it created when a new one is written.
- The backup file is a **plain-text JSON file** containing events, to-dos, day colors, special dates, color label meanings, app settings included in the export, internal identifiers, and backup metadata (such as format version and export time). It is **not encrypted by the app**. Anyone with access to that folder can read its contents. The folder should be chosen accordingly.
- Files are written only to the location chosen by the user. **The developer does not receive, access, or host those files.** If the folder is in a cloud service, that service’s own privacy policy and terms apply.
- Restoring from a backup **replaces** the planner data currently in the app.
- Folder backup may be turned off at any time. Turning it off stops further automatic writes. Existing backup files remain in the folder until the user deletes them.

**User responsibility for backups**

Users are responsible for deciding whether to enable backups and where folder backup files are stored. Because folder backup files are not encrypted by the app, users should choose a storage location they consider appropriate for the information they enter. The developer does not control third-party storage locations (including cloud folders) and cannot guarantee their security or availability. **The developer cannot control or verify the security, privacy, availability, retention, deletion, or backup practices of any storage provider or location selected by the user.** Nothing in this section limits rights or remedies that cannot be excluded under applicable law.

### Feedback emails

The app does not send messages to the developer on its own. If **Feedback** is used, the device email application is opened with a message prepared for the user. To assist troubleshooting, that message is pre-filled with:

- Device manufacturer and model
- Android version (SDK level)
- The Basic Planner version in use (in the email subject)

Nothing is sent unless the message is sent from the user’s own email application. The contents may be edited or deleted first. When a message is sent, the developer receives the sender’s email address, the message, and anything else included (which may include planner content if the sender pastes it). Correspondence is used only to respond to the request and to resolve related issues, is not used for marketing, and is retained only for as long as reasonably necessary for those purposes. Deletion of correspondence may be requested using the contact details below. Email is delivered through the sender’s and the developer’s mail providers, which have their own policies.

### Permissions

The app declares the following permissions. None of them are used to transmit planner content to Basic Organizer or to any server operated by Basic Organizer.

- **INTERNET:** Used only to fetch public holiday data from the Nager.Date API when a holidays country is selected in Settings, as described above.
- **POST_NOTIFICATIONS (Android 13+):** Used to display local reminder notifications when the user has enabled reminders and system notification permission is granted.
- **SCHEDULE_EXACT_ALARM:** Used to schedule local reminder alarms at the times the user chooses. On some Android versions, exact alarms may require an additional allowance in system settings.
- **RECEIVE_BOOT_COMPLETED:** Used to reschedule local reminders after the device restarts.

The scheduling library used for folder backups (AndroidX WorkManager) may add system permissions such as `WAKE_LOCK`, `FOREGROUND_SERVICE`, and `ACCESS_NETWORK_STATE`. These permissions support background scheduling and execution of app operations. They are not used by the developer to upload planner data to developer-operated servers.

Choosing a backup folder uses Android’s system file picker, which grants access only to the location selected. The app does not request broad storage access. Opening an external link (for example the developer page on Google Play) uses the system to launch another application.

### Third-Party Services

The current version of the app contains **no advertising, no analytics, no advertising trackers, no crash-reporting service, and no user accounts**. The libraries it uses (AndroidX and Google Material components) provide user-interface and scheduling functions. They are not used by the developer to collect user data.

If this ever changes, this policy and the app’s Data safety information on Google Play will be updated before the change is released, and consent will be requested where the law requires it.

The following user-initiated actions involve third parties not controlled by Basic Organizer:

- **Feedback:** Opens the device’s email application as described above. Transmission of any message is governed by the email providers’ policies.
- **Developer page on Google Play:** Opens Google Play or a browser. Data processing by Google is governed by [Google’s Privacy Policy](https://policies.google.com/privacy).
- **Google Play distribution:** Installation, updates, ratings, and store interactions involve processing by Google as store operator.
- **Optional Google Backup:** If enabled, device backup that uses the Android backup system is processed by Google as described above.
- **Optional public holidays:** If a country is selected, holiday data is fetched from Nager.Date as described above.

### Data We Do Not Collect

The developer does not operate servers for this app. The app does not transmit planner content to Basic Organizer or to any server operated by Basic Organizer. The following types of information are not transmitted to Basic Organizer or to any server operated by Basic Organizer:

- Event, to-do, or special-date content (except if a user voluntarily includes it in an email)
- Reminder schedules or notification content
- Precise location data
- Contact lists
- Photos, media, or data from other apps
- Advertising identifiers or usage analytics

Google Play, Google Backup, Nager.Date (when used), email providers, Android, and device manufacturers may process information in connection with their respective services under their own policies. The developer does not control those services.

**One exception:** if the user chooses to email the developer (for example through **Feedback**), the developer necessarily receives the email address and whatever is written, as described above. Names, email addresses, and telephone numbers are not otherwise received by the developer.

---

## How We Use Your Information

- Planner data and application preferences remain **local to the device**, unless a backup option is enabled or a holidays country is selected (which triggers the limited API request described above).
- Planner content is not used for advertising or analytics, and is not transmitted to Basic Organizer or to any server operated by Basic Organizer, except if the user includes it in an email.
- When Google Backup or folder backup is enabled, planner data may be copied as described above (Google’s backup systems that use the Android backup system, or a folder chosen by the user). Separate manufacturer transfer tools are described in the backup section.
- When reminders are enabled, reminder scheduling and notifications occur locally on the device.
- Voluntary email is used solely to respond to support inquiries and to resolve related issues.
- Personal information is **not sold**. Personal information is **not shared** for cross-context behavioral advertising.

---

## Data Security

- **Local Storage:** Planner data is stored in a local SQLite database and app-private preferences. Other apps cannot read that storage in ordinary Android use. They may be readable on a rooted or compromised device, or by someone with physical access to an unlocked device.
- **No transmission of planner content to Basic Organizer:** The app does not transmit events, to-dos, special dates, or notes to Basic Organizer or to any server operated by Basic Organizer. The only network use in the app’s own code is the optional public-holidays request described above.
- **Optional backup:** Planner data is added to Google Backup (via the Android backup system) or written as a folder backup only after the corresponding option is enabled in the app.
- **Backup files are not encrypted by the app:** A folder backup is a readable JSON file in the chosen location. Anyone with access to that folder or that cloud account can read it. Google Backup is handled by Google under Google’s own systems and policies. The developer does not control those systems.
- **Reminders:** Reminder alarms and notifications are processed locally. Their reliability depends on device settings and system behavior.
- **Device Security:** Data security also depends on the device’s own protections (screen lock, device encryption, and who has access to the device).
- The app is provided by an independent developer and cannot guarantee absolute security.

---

## Not Professional Advice; Reminders Not Guaranteed

Basic Planner is a personal calendar and planning tool for schedules, to-dos, and dates you choose to record. It is not a professional scheduling service, legal or financial planning service, medical device, or substitute for professional advice.

Optional reminders and calendar displays are provided for convenience only. They may be delayed, skipped, duplicated, or not shown because of permission settings, Do Not Disturb, battery optimization, exact-alarm restrictions, device restart timing, application errors, or other factors outside the developer’s control. **Users should not rely on the app as their only means of remembering critical appointments, deadlines, medications, safety matters, or time-sensitive obligations.**

---

## No Emergency or Safety-Critical Use

Basic Planner is not designed or intended for emergency communications, emergency notifications, safety monitoring, crisis detection, or other safety-critical purposes. Reminders and calendar entries should not be relied upon to identify emergencies or to notify others when assistance may be required.

---

## Data Preservation

The developer does not guarantee that planner data will remain available indefinitely. Data may be lost or become inaccessible due to device failure, operating-system changes, application errors, accidental deletion, uninstallation, storage failure, backup failure, restoration of an earlier backup, device replacement, missed or blocked reminders, or other circumstances outside the developer’s control.

Users are responsible for enabling and maintaining backups if they require copies of their data.

---

## Children's Privacy

- Basic Planner is intended for a general audience. The app is **not directed at children** and is not marketed to children.
- The app is not age-restricted or age-gated. It contains no advertising and no features designed to appeal specifically to children.
- Planner data stays on the device and is not transmitted to Basic Organizer or to any server operated by Basic Organizer through ordinary use of the app. The only way information can reach the developer is if someone chooses to send an email.
- The developer does not knowingly collect personal information from children in circumstances where applicable law requires parental consent or otherwise restricts such collection. If it is believed that a child has sent personal information by email, contact the address below and it will be deleted.

---

## Data Retention and Deletion

- Individual events, to-dos, special dates, and day color marks may be deleted within the application at any time.
- Uninstallation of the application removes locally stored app data under standard Android behavior. **Backups already made are not removed by uninstalling:**
  - Folder backups remain in the chosen folder until the files are deleted (while folder backup is on, the app attempts to keep the 5 newest backup files it created).
  - Google Backup data remains in the Google account until deleted in device or Google account backup settings.
- Cached public-holiday API responses in app-private storage are removed when the app is uninstalled.
- The developer does not operate server-side planner storage.
- Feedback correspondence is retained only for as long as reasonably necessary to respond to the request and resolve related issues. Deletion of correspondence may be requested using the contact details below.

---

## User Rights

- Access, modify, and delete planner data through the application.
- Copy planner data by using folder backup, which writes a JSON file to a chosen folder.
- Opt in or out of optional backup features at any time in Backup & Restore.
- Enable or disable reminders per special date or day to-do, and control notification permission in system settings.
- Users in the EEA, United Kingdom, and Norway may have rights under GDPR / UK GDPR (access, rectification, erasure, portability, objection, complaint to a supervisory authority).

**Who is responsible (GDPR / UK GDPR).** Planner data stays on the device and is not received by the developer, so the developer cannot access, export, or delete planner data on the user’s behalf — that control is exercised directly in the app. For the limited information sent by email, the independent developer who publishes the app under the name Basic Organizer (contact below) acts as the data controller. The legal basis is legitimate interest in answering the message and resolving related issues (GDPR Art. 6(1)(f) / the UK equivalent), or consent where required by law for a particular processing activity (this Privacy Policy is not itself that consent; see Privacy Policy Notice below).

**California (CCPA/CPRA).** Personal information is not sold and is not shared for cross-context behavioral advertising. It is not used to build profiles. California residents may exercise their rights by contacting the address below. There is no discrimination for doing so.

Privacy requests: **basicorganizer.post@gmail.com** (subject: “Privacy request – Basic Planner”), including the nature of the request, jurisdiction, and relevant particulars. GDPR-related requests will be answered within one month where required, with extension by up to two further months where permitted for complex cases.

### Right to Erasure ("Right to be Forgotten")

- Individual events, to-dos, special dates, or day color marks may be deleted within the application
- The application may be uninstalled to remove local app data
- Backup may be turned off, and backup files or device backups that are no longer wanted may be deleted
- The developer may be asked to delete any email correspondence that has been sent
- Because the developer holds no planner data or accounts, there is nothing else to delete on the user’s behalf

---

## Changes to This Privacy Policy

- Updates will be reflected in the "Last Updated" date.
- Material changes will be described in app updates or by in-app notice where practicable.
- If the user does not agree with an updated policy, the application should not continue to be used and may be uninstalled. This policy is a notice of practices; it is not a substitute for rights that cannot be waived under applicable law.

---

## Legal Compliance

This policy is intended to describe the app’s current data practices and has been drafted with commonly applicable privacy and platform requirements in mind, including:

- **GDPR (EEA) and UK GDPR**
- **CCPA/CPRA (California, USA)**
- **COPPA (Children)**
- **Google Play Developer policies**

This is not a certification of compliance with every requirement of every jurisdiction. Laws and store rules change, and an independent developer cannot guarantee that every scenario is covered.

The developer does not receive planner data. For the limited information sent by email, the legal basis is described under User Rights.

International transfer: planner databases are not transferred to developer servers. Email may be processed in jurisdictions where the mail providers operate (which may include countries outside the user’s home country). Optional public-holiday requests are sent to Nager.Date’s servers when a country is selected.

---

## Contact Us

**Email:** basicorganizer.post@gmail.com  
**Published under the name:** Basic Organizer

**Response Time:**
Reasonable efforts will be made to respond to inquiries in a timely manner. For users in the European Economic Area (EEA), the United Kingdom, and Norway, GDPR-related requests will be answered within one month as required by law, and may be extended by up to two further months where necessary, taking into account the complexity and number of requests.

For other inquiries, responses will be provided as promptly as practicable; timing may vary.

When contacting us, please include:
- The concern or request
- Location (jurisdiction), to apply appropriate privacy law
- Relevant details to facilitate handling

---

## Disclaimer

The app and this Privacy Policy are provided "as is" without warranties of any kind. Reasonable efforts are made to protect data and to describe practices accurately; uninterrupted service, timely reminders, or absolute security cannot be guaranteed. Device security, backups, notification settings, and content entered into the app remain the responsibility of the device owner.

The app may calculate, display, summarize, or otherwise present calendar and task information based on data entered by the user. Such information may contain errors, omissions, inaccuracies, or limitations and should not be treated as a guarantee of accuracy. The developer is not responsible for decisions, actions, outcomes, or consequences resulting from reliance on information recorded, displayed, or reminded by the app (including missed reminders).

To the maximum extent permitted by applicable law, Basic Organizer shall not be liable for indirect, incidental, special, consequential, or punitive damages, or for loss of data arising from device failure, third-party services, missed reminders, or circumstances beyond reasonable control. Total liability for claims relating to the app or this policy is limited to amounts paid for the app in the twelve months preceding the claim, or zero if the app was provided without charge, unless mandatory law prohibits such limitation. Some jurisdictions do not allow certain limitations; those provisions apply only to the extent permitted. Nothing in this policy limits rights or remedies that cannot be excluded under consumer or data-protection law.

---

## Privacy Policy Notice

This Privacy Policy is a notice of the app’s privacy practices. It is not, by itself, a request for or a record of consent. Where applicable law requires consent for a particular processing activity (for example showing notifications or enabling backups), that consent is obtained through the relevant system or in-app control, not merely by reading this policy.

---

**Summary:**
- ✓ Planner data stays on the device — the developer does not operate servers for this app
- ✓ Planner content is not transmitted to Basic Organizer or to any server operated by Basic Organizer (only if included in an email the user chooses to send)
- ✓ No ads, analytics, advertising trackers, or accounts in the current version
- ✓ Google Backup and folder backup are optional; both in-app switches start off
- ✓ Folder backup files are readable JSON — they should be kept somewhere trusted
- ✓ Optional public holidays use the Nager.Date API when a supported country applies (country and year in the URL; ordinary network metadata such as IP address may also be visible to that service)
- ✓ Optional local reminders for special dates and day to-dos; not guaranteed; not for emergencies
- ✓ Feedback emails include device model and Android version, and are sent only if the user sends them
- ✓ Planner data can be edited, deleted, or copied (folder backup) in the app
