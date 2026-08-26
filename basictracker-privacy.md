# Privacy Policy for Basic Tracker

**Last Updated: August 26, 2026**

## Introduction

This Privacy Policy explains how Basic Tracker ("we", "our", or "the app") collects, uses, and handles information in connection with the Android mobile application (package name: `com.basicorganizer.tracker`).

This policy covers the Basic Tracker Android application published by Basic Organizer. It does not govern Google Play, email providers, Google’s backup systems, device manufacturers, or other third-party services. Those parties have their own policies.

Basic Organizer develops and maintains the app as an independent project. The application does not operate developer-run servers and does not upload tracking content to the developer. This document is provided for transparency and does not constitute legal advice.

## Developer Information

**App Name:** Basic Tracker (device label: Tracker)  
**Developer:** Basic Organizer  
**Contact Email:** basicorganizer.post@gmail.com  
**Distribution:** Google Play Store

**Note:** This app is developed and maintained as an independent project. While we strive to provide reliable service and support, response times and feature development may vary based on available resources.

## Information We Collect

### Data Stored Locally

All application data required for operation is stored **locally on the device**:

- **Tracking items:** Names, sentiment (positive / negative / neutral), display order, archive status, and creation dates
- **Tracking entries:** Which days were marked for each item, including optional time of day when a mark is recorded
- **Day notes:** Text notes attached to specific items and dates
- **App Preferences:** Default item designation; language preference (including system default); first day of the week; theme (light / dark); backup choices (including the backup folder selected, if any)

This information is stored in a local SQLite database and in app-private preferences. The app does **not** send it to the developer or to any server operated by the developer.

Item names, day notes, and other text entered by the user may constitute personal or sensitive information depending on content. Users are responsible for the information they choose to enter into the app, including determining whether such information is appropriate to store on their device or in any backup location. Users should not use the app to store information that they are legally prohibited from storing, information belonging to another person without appropriate authorization, passwords, authentication credentials, financial credentials, or other information requiring a level of security that the app does not provide. The developer does not use user-entered content for advertising or analytics.

### Optional backups

Backup is **optional**. In the app, both Google Backup and folder backup are **off by default** until switched on in **Backup & Restore**. Either option, both, or neither may be used.

**Google Backup**

- The app allows Android backup (`allowBackup`), but tracking data is included in a backup that uses the Android backup system only when the in-app Google Backup option is enabled. A custom backup agent includes the tracking database and backup settings only when that option is switched on; if it is off, the agent backs up nothing.
- Tracking data is added to Google Backup only when the Google Backup option is switched on in **Backup & Restore** *and* Google Backup is enabled in device settings. That backup includes the tracking database and backup preference settings (such as opt-in flags and, if folder backup was configured, the chosen folder location). Other app preferences (for example language, first day of week, theme, and default item) are not included in that backup.
- That backup is handled by Google under [Google’s Privacy Policy](https://policies.google.com/privacy), not by the Basic Tracker developer. **The developer does not receive, access, or host that data.**
- The option may be turned off in the app at any time. Turning it off stops the app from adding tracking data to later backups that use the Android backup system. Copies already stored by Google remain until deleted in Google account or device backup settings.
- The app’s backup configuration applies to backup mechanisms that use the Android backup system. Device manufacturers may provide separate transfer or migration tools whose behaviour can vary by device and Android version and which may be governed by the manufacturer’s own settings and policies.
- The developer does not control third-party device backup, migration, cloning, synchronization, restoration, or transfer mechanisms. Such mechanisms may copy, retain, modify, omit, or otherwise process application data independently of the app’s own backup settings. Their operation is governed by the applicable device manufacturer, operating system, or service provider.

**Folder backup**

- Only when switched on and a folder is chosen with the system file picker (for example a folder on the device, or in the user’s own cloud storage).
- When folder backup is enabled, a backup file is written promptly, then about once a day (the schedule may be delayed if the battery is low). The app attempts to keep the **5 most recent** backup files it created in that folder and may delete older backup files it created when a new one is written.
- The backup file is a **plain-text JSON file** containing tracking items (including archived items), tracking entries (including optional times), day notes, internal identifiers, and backup metadata (such as format version and export time). It is **not encrypted by the app**. Anyone with access to that folder can read its contents. The folder should be chosen accordingly.
- Files are written only to the location chosen by the user. **The developer does not receive, access, or host those files.** If the folder is in a cloud service, that service’s own privacy policy and terms apply.
- Restoring from a backup **replaces** the tracking data currently in the app.
- Folder backup may be turned off at any time. Turning it off stops further automatic writes. Existing backup files remain in the folder until the user deletes them.

**User responsibility for backups**

Users are responsible for deciding whether to enable backups and where folder backup files are stored. Because folder backup files are not encrypted by the app, users should choose a storage location they consider appropriate for the information they enter. The developer does not control third-party storage locations (including cloud folders) and cannot guarantee their security or availability. **The developer cannot control or verify the security, privacy, availability, retention, deletion, or backup practices of any storage provider or location selected by the user.** Nothing in this section limits rights or remedies that cannot be excluded under applicable law.

### Feedback emails

The app does not send messages to the developer on its own. If **Feedback** is used, the device email application is opened with a message prepared for the user. To assist troubleshooting, that message is pre-filled with:

- Device manufacturer and model
- Android version (SDK level)
- The Basic Tracker version in use (in the email subject)

Nothing is sent unless the message is sent from the user’s own email application. The contents may be edited or deleted first. When a message is sent, the developer receives the sender’s email address, the message, and anything else included (which may include tracking content if the sender pastes it). Correspondence is used only to respond to the request and to resolve related issues, is not used for marketing, and is retained only for as long as reasonably necessary for those purposes. Deletion of correspondence may be requested using the contact details below. Email is delivered through the sender’s and the developer’s mail providers, which have their own policies.

### Permissions

The app does **not** declare the Android internet permission, and the application code does not upload tracking data to the developer.

The app uses Android system functionality to schedule local backup operations (AndroidX WorkManager). WorkManager may add system permissions such as `WAKE_LOCK`, `RECEIVE_BOOT_COMPLETED`, `FOREGROUND_SERVICE`, and `ACCESS_NETWORK_STATE`; these are used only to schedule and run local folder backups on the device, not to upload tracking data to the developer.

Choosing a backup folder uses Android’s system file picker, which grants access only to the location selected. The app does not request broad storage access. Opening an external link (for example the developer page on Google Play) uses the system to launch another application; it does not grant this app network access.

### Third-Party Services

The current version of the app contains **no advertising, no analytics, no advertising trackers, no crash-reporting service, and no user accounts**. The libraries it uses (AndroidX and Google Material components) provide user-interface and scheduling functions. They are not used by the developer to collect user data.

If this ever changes, this policy and the app’s Data safety information on Google Play will be updated before the change is released, and consent will be requested where the law requires it.

The following user-initiated actions involve third parties not controlled by Basic Organizer:

- **Feedback:** Opens the device’s email application as described above. Transmission of any message is governed by the email providers’ policies.
- **Developer page on Google Play:** Opens Google Play or a browser. Data processing by Google is governed by [Google’s Privacy Policy](https://policies.google.com/privacy).
- **Google Play distribution:** Installation, updates, ratings, and store interactions involve processing by Google as store operator.
- **Optional Google Backup:** If enabled, device backup that uses the Android backup system is processed by Google as described above.

### Data We Do Not Collect

The developer does not operate servers for this app. The app does not send data to the developer by itself. Through the app, the following are not sent to the developer:

- Tracking item names, entries, or day notes
- Precise location data
- Contact lists
- Photos, media, or data from other apps
- Advertising identifiers or usage analytics

Google Play, Google Backup, email providers, Android, and device manufacturers may process information in connection with their respective services under their own policies. The developer does not control those services.

**One exception:** if the user chooses to email the developer (for example through **Feedback**), the developer necessarily receives the email address and whatever is written, as described above. Names, email addresses, and telephone numbers are not otherwise received by the developer.

---

## How We Use Your Information

- Tracking data and application preferences remain **local to the device**, unless a backup option is enabled as described above.
- Tracking content is not used for advertising or analytics, and is not sent to the developer except if the user includes it in an email.
- When Google Backup or folder backup is enabled, tracking data may be copied as described above (Google’s backup systems that use the Android backup system, or a folder chosen by the user). Separate manufacturer transfer tools are described in the backup section.
- Voluntary email is used solely to respond to support inquiries and to resolve related issues.
- Personal information is **not sold**. Personal information is **not shared** for cross-context behavioural advertising.

---

## Data Security

- **Local Storage:** Tracking data is stored in a local SQLite database in the app’s private storage. Other apps cannot read that storage in ordinary Android use. They may be readable on a rooted or compromised device, or by someone with physical access to an unlocked device.
- **No upload by the app:** The app does not declare internet permission and does not upload tracking data to the developer.
- **Optional backup:** Tracking data is added to Google Backup (via the Android backup system) or written as a folder backup only after the corresponding option is enabled in the app.
- **Backup files are not encrypted by the app:** A folder backup is a readable JSON file in the chosen location. Anyone with access to that folder or that cloud account can read it. Google Backup is handled by Google under Google’s own systems and policies. The developer does not control those systems.
- **Device Security:** Data security also depends on the device’s own protections (screen lock, device encryption, and who has access to the device).
- The app is provided by an independent developer and cannot guarantee absolute security.

---

## Not Medical or Mental-Health Advice

Basic Tracker is a personal tracking and journaling tool for habits, routines, and other information you choose to record. It is not a medical device, healthcare service, diagnostic tool, treatment tool, or mental-health service, and it does not provide medical, psychological, or professional advice — even if you use it to log symptoms, moods, or other health-related topics of your own choosing.

Any statistics, trends, summaries, patterns, sentiment classifications, or other information generated by the app are provided for informational and personal-record-keeping purposes only. They may be incomplete, inaccurate, or unsuitable for making medical, mental-health, safety, financial, or other important decisions.

Users should not rely on the app to diagnose, treat, monitor, prevent, or manage any medical or mental-health condition. If you have concerns about your health, mental health, safety, or wellbeing, consult an appropriately qualified professional.

The app is not intended to replace professional advice, diagnosis, treatment, or emergency services.

---

## No Emergency or Safety-Critical Use

Basic Tracker is not designed or intended for emergency communications, emergency notifications, safety monitoring, crisis detection, or other safety-critical purposes. The app should not be relied upon to identify emergencies, detect dangerous conditions, or notify another person when assistance may be required.

---

## Data Preservation

The developer does not guarantee that tracking data will remain available indefinitely. Data may be lost or become inaccessible due to device failure, operating-system changes, application errors, accidental deletion, uninstallation, storage failure, backup failure, restoration of an earlier backup, device replacement, or other circumstances outside the developer’s control.

Users are responsible for enabling and maintaining backups if they require copies of their data.

---

## Children's Privacy

- Basic Tracker is intended for a general audience. The app is **not directed at children** and is not marketed to children.
- The app is not age-restricted or age-gated. It contains no advertising and no features designed to appeal specifically to children.
- Tracking data stays on the device and is not sent to the developer through ordinary use of the app. The only way information can reach the developer is if someone chooses to send an email.
- The developer does not knowingly collect personal information from children in circumstances where applicable law requires parental consent or otherwise restricts such collection. If it is believed that a child has sent personal information by email, contact the address below and it will be deleted.

---

## Data Retention and Deletion

- Individual tracking items, entries, and day notes may be deleted within the application at any time. Archived items remain on the device until unarchived or deleted.
- Uninstallation of the application removes locally stored app data under standard Android behaviour. **Backups already made are not removed by uninstalling:**
  - Folder backups remain in the chosen folder until the files are deleted (while folder backup is on, the app attempts to keep the 5 newest backup files it created).
  - Google Backup data remains in the Google account until deleted in device or Google account backup settings.
- The developer does not operate server-side tracking storage.
- Feedback correspondence is retained only for as long as reasonably necessary to respond to the request and resolve related issues. Deletion of correspondence may be requested using the contact details below.

---

## User Rights

- Access, modify, and delete tracking data through the application.
- Copy tracking data by using folder backup, which writes a JSON file to a chosen folder.
- Opt in or out of optional backup features at any time in Backup & Restore.
- Users in the EEA, United Kingdom, and Norway may have rights under GDPR / UK GDPR (access, rectification, erasure, portability, objection, complaint to a supervisory authority).

**Who is responsible (GDPR / UK GDPR).** Tracking data stays on the device and is not received by the developer, so the developer cannot access, export, or delete tracking data on the user’s behalf — that control is exercised directly in the app. For the limited information sent by email, the independent developer who publishes the app under the name Basic Organizer (contact below) acts as the data controller. The legal basis is legitimate interest in answering the message and resolving related issues (GDPR Art. 6(1)(f) / the UK equivalent), or consent where required by law for a particular processing activity (this Privacy Policy is not itself that consent; see Privacy Policy Notice below).

**California (CCPA/CPRA).** Personal information is not sold and is not shared for cross-context behavioural advertising. It is not used to build profiles. California residents may exercise their rights by contacting the address below. There is no discrimination for doing so.

Privacy requests: **basicorganizer.post@gmail.com** (subject: “Privacy request – Basic Tracker”), including the nature of the request, jurisdiction, and relevant particulars. GDPR-related requests will be answered within one month where required, with extension by up to two further months where permitted for complex cases.

### Right to Erasure ("Right to be Forgotten")

- Individual tracking items, entries, or day notes may be deleted within the application
- The application may be uninstalled to remove local app data
- Backup may be turned off, and backup files or device backups that are no longer wanted may be deleted
- The developer may be asked to delete any email correspondence that has been sent
- Because the developer holds no tracking data or accounts, there is nothing else to delete on the user’s behalf

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

The developer does not receive tracking data. For the limited information sent by email, the legal basis is described under User Rights.

International transfer: tracking databases are not transferred to developer servers. Email may be processed in jurisdictions where the mail providers operate (which may include countries outside the user’s home country).

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

The app and this Privacy Policy are provided "as is" without warranties of any kind. Reasonable efforts are made to protect data and to describe practices accurately; uninterrupted service or absolute security cannot be guaranteed. Device security, backups, and content entered into the app remain the responsibility of the device owner.

The app may calculate, display, summarize, categorize, or otherwise present information based on data entered by the user. Such information may contain errors, omissions, inaccuracies, or limitations and should not be treated as a guarantee of accuracy. The developer is not responsible for decisions, actions, outcomes, or consequences resulting from reliance on information recorded, calculated, displayed, or summarized by the app.

To the maximum extent permitted by applicable law, Basic Organizer shall not be liable for indirect, incidental, special, consequential, or punitive damages, or for loss of data arising from device failure, third-party services, or circumstances beyond reasonable control. Total liability for claims relating to the app or this policy is limited to amounts paid for the app in the twelve months preceding the claim, or zero if the app was provided without charge, unless mandatory law prohibits such limitation. Some jurisdictions do not allow certain limitations; those provisions apply only to the extent permitted. Nothing in this policy limits rights or remedies that cannot be excluded under consumer or data-protection law.

---

## Privacy Policy Notice

This Privacy Policy is a notice of the app’s privacy practices. It is not, by itself, a request for or a record of consent. Where applicable law requires consent for a particular processing activity, that consent will be obtained separately.

---

**Summary:**
- ✓ Tracking data stays on the device — the app does not declare internet permission and the developer does not operate servers for this app
- ✓ Tracking content is not sent to the developer by the app (only if included in an email the user chooses to send)
- ✓ No ads, analytics, advertising trackers, or accounts in the current version
- ✓ Google Backup and folder backup are optional; both in-app switches start off
- ✓ Folder backup files are readable JSON — they should be kept somewhere trusted
- ✓ Feedback emails include device model and Android version, and are sent only if the user sends them
- ✓ Tracking data can be edited, deleted, or copied (folder backup) in the app
- ✓ Not medical / mental-health advice; not for emergency or safety-critical use
