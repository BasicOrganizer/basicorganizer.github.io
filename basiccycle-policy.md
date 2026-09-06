# Privacy Policy for Basic Cycle

**Last Updated: September 6, 2026**

## Introduction

This Privacy Policy explains how Basic Cycle ("we", "our", or "the app") handles information in connection with the Android mobile application (package name: `com.basicorganizer.cycle`).

**Basic Cycle stores information you enter locally on your device. The developer does not receive or have access to that information through the app.** Optional backups and voluntary emails are described separately below.

This policy covers the Basic Cycle Android application published by Basic Organizer. It does not govern Google Play, email providers, Google's backup systems, device manufacturers, or other third-party services. Those parties have their own policies.

Basic Organizer develops and maintains the app as an independent project. The application does not operate developer-run servers. Cycle, health, intimacy, or other content you enter is **not transmitted by the app** to Basic Organizer or to any server operated by Basic Organizer. This document is provided for transparency and does not constitute legal advice.

## Developer Information

**App Name:** Basic Cycle (device label: Cycle)  
**Developer:** Basic Organizer  
**Contact Email:** basicorganizer.post@gmail.com  
**Distribution:** Google Play Store

**Note:** This app is developed and maintained as an independent project. While we strive to provide reliable service and support, response times and feature development may vary based on available resources.

---

## Not Medical Advice; Not a Contraceptive; Predictions Not Guaranteed

Basic Cycle is a personal period and menstrual-cycle tracking tool for information you choose to record. It is **not a medical device**, healthcare service, diagnostic tool, treatment tool, fertility clinic, or contraceptive method, and it does **not** provide medical, fertility, pregnancy, or professional advice.

**Do not rely on this app or its predictions for contraception, pregnancy prevention, conception, fertility treatment, family planning, or any other medical or reproductive decision.**

Cycle predictions, fertile-window estimates, ovulation estimates, period-delay estimates, statistics, calendar markers, toolbar status text, and optional morning notifications are automatically generated estimates based only on the information you enter and on simple local algorithms. They may be incomplete, inaccurate, delayed, skipped, or unsuitable for decision-making — especially with irregular cycles, illness, PCOS, postpartum changes, hormonal contraception, incomplete logging, or other factors. **It remains possible to become pregnant on days outside any predicted fertile window.**

Users should not rely on the app as their only means of remembering periods, fertile days, medical appointments, medications, or other time-sensitive matters. If you have concerns about your health, fertility, pregnancy, or contraception, consult an appropriately qualified healthcare professional.

The app is not intended to replace professional advice, diagnosis, treatment, emergency services, or clinically validated fertility-awareness or contraceptive methods.

Basic Cycle is **not** a healthcare provider, health insurer, or other entity covered by the U.S. Health Insurance Portability and Accountability Act (HIPAA), and this policy is not a HIPAA notice.

---

## Health and Sensitive Information

Information you enter into Basic Cycle — including menstrual cycles, period days, ovulation, symptoms, notes, intimacy (sexual activity), and related preferences — may be considered **sensitive personal information** or health-related information under certain laws (including special-category data under GDPR / UK GDPR where applicable).

This information is stored **locally on your device** by default and is **not transmitted by the app** to Basic Organizer or to any server operated by Basic Organizer. Optional backup features can create copies outside the app's private storage, as described below. Optional morning notifications may display cycle-related text on the device notification shade when enabled and permitted by the system.

Health-related information is used by the app to provide tracking, calendar, journal, statistics, personalization, optional reminders, and related functionality. It may also be included in optional backups enabled by the user or in communications the user voluntarily sends to the developer. It is **never** used for advertising, profiling, analytics, marketing, or sold or shared with third parties by the developer.

Basic Cycle does **not** use artificial intelligence or external cloud services to analyze your health information. Calculations and predictions run **locally on your device**.

Users are responsible for the information they choose to enter, including whether it is appropriate to store on their device or in any backup location. Users should not use the app to store information that they are legally prohibited from storing, information belonging to another person without appropriate authorization, passwords, authentication credentials, financial credentials, or other information requiring a level of security that the app does not provide.

---

## No Emergency or Safety-Critical Use

Basic Cycle is not designed or intended for emergency communications, emergency notifications, safety monitoring, crisis detection, pregnancy emergency detection, or other safety-critical purposes. Optional notifications and calendar displays should not be relied upon to identify emergencies or to notify others when assistance may be required.

---

## Information Stored in the App

In this policy, "stored" means information kept in the app's local storage on the device for the app to function. That is **not** the same as information being received, accessed, or collected by Basic Organizer. Unless this policy expressly says otherwise (for example optional backups or a voluntary email), Basic Organizer does not receive that information.

### Data Stored Locally

Application data required for ordinary operation is stored **locally on the device**:

- **Cycle log:** Days marked as period days and days marked as ovulation
- **Symptoms:** Symptoms logged on specific dates, including custom symptoms you create and which predefined symptoms are shown or hidden
- **Intimacy records:** Days you choose to mark intimacy (sexual activity)
- **Notes:** Free-text notes associated with specific dates
- **Personalization:** Typical cycle length, period length, and whether predictions use your logged averages and/or tracked ovulation
- **Calendar display preferences:** Which predicted markers to show (for example predicted period, cycle variation, predicted ovulation, predicted fertile days)
- **Notification preferences:** Which categories of optional morning reminders are enabled (upcoming period, period delay, fertility window and ovulation), and related local scheduling state
- **App preferences:** Language (including system default); first day of the week; theme (light / dark / system); optional app PIN (stored as a salted hash, not the PIN itself); disclaimer acknowledgement; and backup choices (including the backup folder selected, if any)

This information is stored in a local SQLite database and in app-private SharedPreferences. The app does **not** transmit it to Basic Organizer or to any server operated by Basic Organizer. Optional backup features can create copies of this data outside the device, as described in the backup section below.

### Optional morning notifications

Morning cycle reminders are **optional**. Categories can be turned on or off in **Notifications**. By default, the in-app category switches start **on**, but notifications appear on screen only if the device's notification permission / system notification settings also allow them.

When a category is enabled and the system allows notifications, the app may schedule a **local** morning reminder for **approximately 8:00 local time, subject to Android's background scheduling and device power-management behavior**, and show at most one notification on a given day when a matching cycle condition applies, such as:

- Upcoming period milestones (including the start of the luteal phase and selected days before a predicted period, or period expected today)
- Period delay (including daily reminders while a predicted period is late, up to a capped number of days)
- Fertile-window and predicted ovulation reminders

Notification text is derived from the same local prediction logic used in the calendar and may include cycle-related wording. **Notification content is not transmitted by the app to Basic Organizer or to any server operated by Basic Organizer.**

On Android 13 and later, the app declares the **POST_NOTIFICATIONS** permission. The Notifications screen may show a message with a link to system settings if notifications are not enabled; the app does not automatically force a permission prompt when saving. If permission is denied, or if notifications are blocked in system settings, reminders may not appear even though the in-app category switches remain on.

After a device restart or app update, the app may reschedule the next morning reminder locally. Delivery can be affected by Do Not Disturb, battery optimization, Doze mode, WorkManager timing, manufacturer-specific power management, timezone changes, missing or incomplete cycle data, or other system settings outside the developer's control. **Notifications are not guaranteed to fire at the exact intended moment, or at all.**

Tapping a notification opens the app. No third-party analytics or advertising SDK receives notification events through the app.

### Optional app PIN (app lock)

An optional numeric PIN may be set in **Settings**. When enabled, the app may require the PIN when the app is opened or returned to from the background.

- The PIN itself is **not stored**. The app stores a **salted cryptographic hash** of the PIN in app-private preferences.
- The PIN is a convenience lock for casual access on the device. It is **not** a guarantee of security against a determined attacker, rooted or compromised devices, backups, forensic tools, or physical access to an unlocked device.
- If folder backup is enabled and a PIN is set, **the salted hash and salt are included in the backup file** so the lock can be restored. Anyone with access to that backup file can see that a PIN lock is configured and may attempt offline attacks against the hash. Choose backup locations accordingly.
- Forgotten PINs cannot be recovered by the developer. Clearing app data or restoring a backup without the PIN hash (or uninstalling without a usable backup) may be required to regain access, which can result in data loss if no suitable backup exists.

### Optional backups

Backup is **optional**. In the app, both Google Backup and folder backup are **off by default** until switched on in **Backup & Restore**. Either option, both, or neither may be used.

Because cycle data may include sensitive health and intimacy information, users should consider carefully whether to enable backups and where folder backup files are stored.

**Google Backup**

- The app allows Android backup (`allowBackup`), but cycle data is included in a backup that uses the Android backup system only when the in-app Google Backup option is enabled. A custom backup agent includes the cycle database and related preference files only when that option is switched on; if it is off, the agent backs up nothing.
- Cycle data is added to Google Backup only when the Google Backup option is switched on in **Backup & Restore** *and* Google Backup is enabled in device settings. When included, that backup contains:
  - The cycle SQLite database (period days, ovulation days, intimacy days, notes, symptoms, and custom symptoms)
  - App preferences (including personalization, display preferences, notification category switches, theme, language-related preferences stored there, disclaimer acknowledgement, symptom visibility, and PIN hash/salt if a PIN is set)
  - Backup preference settings (such as opt-in flags and, if folder backup was configured, the chosen folder location)
- That backup is handled by Google under [Google's Privacy Policy](https://policies.google.com/privacy), not by the Basic Cycle developer. **The developer does not receive, access, or host that data.** **Basic Organizer does not control Google's encryption, retention, restoration, or deletion mechanisms for Google Backup.**
- The option may be turned off in the app at any time. Turning it off stops the app from adding cycle data to later backups that use the Android backup system. Copies already stored by Google remain until deleted in Google account or device backup settings.
- The app's backup configuration applies to backup mechanisms that use the Android backup system. Device manufacturers may provide separate transfer or migration tools whose behavior can vary by device and Android version and which may be governed by the manufacturer's own settings and policies.
- The developer does not control third-party device backup, migration, cloning, synchronization, restoration, or transfer mechanisms. Such mechanisms may copy, retain, modify, omit, or otherwise process application data independently of the app's own backup settings. Their operation is governed by the applicable device manufacturer, operating system, or service provider.

**Folder backup**

- Only when switched on and a folder is chosen with the system file picker (for example a folder on the device, or in the user's own cloud storage).
- When folder backup is enabled, a backup file is written promptly, then about once a day (the schedule may be delayed if the battery is low). The app attempts to keep the **5 most recent** backup files it created in that folder and may delete older backup files it created when a new one is written.
- The backup file is a **plain-text JSON file** containing period days, ovulation days, intimacy days, notes, symptoms, custom symptoms, exported preferences (including personalization, calendar prediction display options, notification category switches, theme, disclaimer acknowledgement, symptom visibility, and PIN salt/hash if a PIN is set), and backup metadata (such as format version and export time). It is **not encrypted by the app**. Anyone with access to that folder can read its contents, which may include sensitive health and intimacy information. The folder should be chosen accordingly.
- Files are written only to the location chosen by the user. **The developer does not receive, access, or host those files.** If the folder is in a cloud service, that service's own privacy policy and terms apply.
- Restoring from a backup **replaces** the cycle data currently in the app.
- Folder backup may be turned off at any time. Turning it off stops further automatic writes. Existing backup files remain in the folder until the user deletes them.

**User responsibility for backups**

Users are responsible for deciding whether to enable backups and where folder backup files are stored. Because folder backup files are not encrypted by the app and may contain sensitive health and intimacy information, users should choose a storage location they consider appropriate. The developer does not control third-party storage locations (including cloud folders) and cannot guarantee their security or availability. **The developer cannot control or verify the security, privacy, availability, retention, deletion, or backup practices of any storage provider or location selected by the user.** Nothing in this section limits rights or remedies that cannot be excluded under applicable law.

### Feedback emails

The app does not send messages to the developer on its own. If **Feedback** is used, the device email application is opened with a message prepared for the user. To assist troubleshooting, that message is pre-filled with:

- Device manufacturer and model
- Android version (SDK level)
- The Basic Cycle version in use (in the email subject)

Nothing is sent unless the message is sent from the user's own email application. The contents may be edited or deleted first. When a message is sent, the developer receives the sender's email address, the message, and anything else included (which may include cycle or health content if the sender pastes it). Correspondence is used only to respond to the request and to resolve related issues, is not used for marketing, and is retained only for as long as reasonably necessary for those purposes. Deletion of correspondence may be requested using the contact details below. Email is delivered through the sender's and the developer's mail providers, which have their own policies.

### Permissions

The app declares the following permissions. None of them are used by the app to transmit cycle content to Basic Organizer or to any server operated by Basic Organizer.

- **POST_NOTIFICATIONS (Android 13+):** Used to display optional local morning cycle reminders when the user has enabled notification categories and system notification permission is granted.
- **RECEIVE_BOOT_COMPLETED:** Used to reschedule the next local morning reminder after the device restarts (and after the app is updated, where applicable).

The app does **not** declare the Android **INTERNET** permission, and the application code does not upload cycle data to the developer.

The scheduling library used for folder backups and morning reminders (AndroidX WorkManager) may add system permissions such as `WAKE_LOCK`, `FOREGROUND_SERVICE`, and `ACCESS_NETWORK_STATE`. These permissions support background scheduling and execution of app operations on the device. They are not used by the developer to upload cycle data to developer-operated servers.

Choosing a backup folder uses Android's system file picker, which grants access only to the location selected. The app does not request broad storage access. Opening an external link (for example the developer page on Google Play) uses the system to launch another application; it does not grant this app network access for uploading cycle data.

### Third-Party Services

The current version of the app contains **no advertising, no analytics, no advertising trackers, no crash-reporting service, and no user accounts**. The libraries it uses (AndroidX and Google Material components) provide user-interface and scheduling functions. They are not used by the developer to collect user data.

If this ever changes, this policy and the app's Data safety information on Google Play will be updated before the change is released, and consent will be requested where the law requires it.

The following user-initiated actions involve third parties not controlled by Basic Organizer:

- **Feedback:** Opens the device's email application as described above. Transmission of any message is governed by the email providers' policies.
- **Developer page on Google Play:** Opens Google Play or a browser. Data processing by Google is governed by [Google's Privacy Policy](https://policies.google.com/privacy).
- **Google Play distribution:** Installation, updates, ratings, and store interactions involve processing by Google as store operator.
- **Optional Google Backup:** If enabled, device backup that uses the Android backup system is processed by Google as described above.

### Information the Developer Does Not Receive Through the App

The developer does not operate servers for this app. Through ordinary use of the app, the following are **not transmitted by the app** to Basic Organizer or to any server operated by Basic Organizer:

- Period, ovulation, intimacy, symptom, or note content
- Prediction inputs, statistics, or notification content
- Precise location data
- Contact lists
- Photos, media, or data from other apps
- Advertising identifiers or usage analytics

Google Play, Google Backup, email providers, Android, and device manufacturers may process information in connection with their respective services under their own policies. The developer does not control those services.

**User-initiated email is different:** if the user chooses to email the developer (for example through **Feedback**), the developer necessarily receives the email address and whatever is written, as described above. Names, email addresses, and telephone numbers are not otherwise received by the developer through the app.

---

## How We Use Your Information

- Cycle data and application preferences remain **local to the device**, unless a backup option is enabled as described above.
- Cycle content is not used for advertising or analytics, and is not transmitted **by the app** to Basic Organizer or to any server operated by Basic Organizer, except if the user includes it in an email.
- When Google Backup or folder backup is enabled, cycle data may be copied as described above (Google's backup systems that use the Android backup system, or a folder chosen by the user). Separate manufacturer transfer tools are described in the backup section.
- When notification categories are enabled and system permission allows it, reminder scheduling and notifications occur locally on the device.
- Voluntary email is used only to respond to support inquiries and to resolve related issues.
- Personal information is **not sold**. Personal information is **not shared** for cross-context behavioral advertising.

---

## Data Security

- **Local Storage:** Cycle data is stored in a local SQLite database and app-private preferences. Other apps cannot read that storage in ordinary Android use. They may be readable on a rooted or compromised device, or by someone with physical access to an unlocked device.
- **No upload by the app:** The app does not declare internet permission and does not transmit period, ovulation, intimacy, symptom, or note content to Basic Organizer or to any server operated by Basic Organizer.
- **Optional backup:** Cycle data is added to Google Backup (via the Android backup system) or written as a folder backup only after the corresponding option is enabled in the app.
- **Backup files are not encrypted by the app:** A folder backup is a readable JSON file in the chosen location. Anyone with access to that folder or that cloud account can read it, including sensitive health and intimacy information if present. Google Backup is handled by Google under Google's own systems and policies. The developer does not control those systems.
- **Optional PIN:** The PIN lock is a convenience feature. It is not a substitute for device screen lock, full-disk encryption, or professional security controls.
- **Notifications:** Reminder scheduling and notifications are processed locally. Their reliability depends on device settings and system behavior.
- **Device Security:** Data security also depends on the device's own protections (screen lock, device encryption, and who has access to the device).
- The app is provided by an independent developer and cannot guarantee absolute security.

---

## Data Preservation

The developer does not guarantee that cycle data will remain available indefinitely. Data may be lost or become inaccessible due to device failure, operating-system changes, application errors, accidental deletion, uninstallation, storage failure, backup failure, restoration of an earlier backup, device replacement, forgotten PIN without a usable backup, missed or blocked notifications, or other circumstances outside the developer's control.

Users are responsible for enabling and maintaining backups if they require copies of their data.

---

## Children's Privacy

- Basic Cycle is intended for people who wish to track menstrual cycles. The app is **not directed at children** and is not marketed to children.
- The app is not age-restricted or age-gated. It contains no advertising and no features designed to appeal specifically to children.
- Cycle data stays on the device and is not transmitted **by the app** to Basic Organizer or to any server operated by Basic Organizer through ordinary use of the app. The only way information can reach the developer is if someone chooses to send an email.
- The developer does not knowingly collect personal information from children in circumstances where applicable law requires parental consent or otherwise restricts such collection. If it is believed that a child has sent personal information by email, contact the address below and it will be deleted.

---

## Data Retention and Deletion

- Individual period days, ovulation days, intimacy marks, symptoms, notes, and custom symptoms may be deleted or unmarked within the application at any time.
- Uninstallation of the application removes locally stored app data under standard Android behavior. **Backups already made are not removed by uninstalling:**
  - Folder backups remain in the chosen folder until the files are deleted (while folder backup is on, the app attempts to keep the 5 newest backup files it created).
  - Google Backup data remains in the Google account until deleted in device or Google account backup settings.
- The developer does not operate server-side cycle storage.
- Feedback correspondence is retained only for as long as reasonably necessary to respond to the request and resolve related issues. Deletion of correspondence may be requested using the contact details below.

---

## User Rights

- Access, modify, and delete cycle data through the application.
- Copy cycle data by using folder backup, which writes a JSON file to a chosen folder.
- Opt in or out of optional backup features at any time in Backup & Restore.
- Enable or disable notification categories in Notifications, and control notification permission in system settings.
- Set, change, or remove an optional app PIN in Settings.
- Users in the EEA, United Kingdom, and Norway may have rights under GDPR / UK GDPR (access, rectification, erasure, portability, objection, complaint to a supervisory authority), including rights relating to special-category / health data where applicable.

**Who is responsible (GDPR / UK GDPR).** Cycle data stays on the device and is not received by the developer through the app, so the developer cannot access, export, or delete cycle data on the user's behalf — that control is exercised directly in the app. For information voluntarily sent by email, the independent developer who publishes the app under the name Basic Organizer (contact below) acts as the data controller. For that information, the developer determines the applicable legal basis under the circumstances, which may include legitimate interests for responding to an inquiry and, where special-category data or another form of consent is involved, an applicable condition under Article 9 GDPR / the corresponding UK GDPR requirements (this Privacy Policy is not itself that consent; see Privacy Policy Notice below).

**California (CCPA/CPRA).** Personal information is not sold and is not shared for cross-context behavioral advertising. It is not used to build profiles. California residents may exercise their rights by contacting the address below. There is no discrimination for doing so. The categories of sensitive personal information that may be stored locally by the app, and the circumstances in which information may leave the device through user-enabled backups or voluntary communications, are described in this policy.

Privacy requests: **basicorganizer.post@gmail.com** (subject: "Privacy request - Basic Cycle"), including the nature of the request, jurisdiction, and relevant particulars. GDPR-related requests will be answered within one month where required, with extension by up to two further months where permitted for complex cases.

### Right to Erasure ("Right to be Forgotten")

- Individual cycle entries, symptoms, notes, or custom symptoms may be deleted within the application
- The application may be uninstalled to remove local app data
- Backup may be turned off, and backup files or device backups that are no longer wanted may be deleted
- The developer may be asked to delete any email correspondence that has been sent
- Because the developer does not hold cycle data or user accounts, there is no developer-held cycle database to delete. Any personal information contained in support correspondence can be handled as described in the Feedback emails and Data Retention sections.

---

## Changes to This Privacy Policy

- Updates will be reflected in the "Last Updated" date.
- Material changes will be described in app updates or by in-app notice where practicable.
- If the user does not agree with an updated policy, the application should not continue to be used and may be uninstalled. This policy is a notice of practices; it is not a substitute for rights that cannot be waived under applicable law.

---

## Legal Compliance

This policy is intended to describe the app's current data practices and has been drafted with commonly applicable privacy and platform requirements in mind, including:

- **GDPR (EEA) and UK GDPR**
- **CCPA/CPRA (California, USA)**
- **COPPA (Children)**
- **Google Play Developer policies**, including Google Play's User Data policy and Health Apps policy, as applicable to the app's health-related functionality

This is not a certification of compliance with every requirement of every jurisdiction. Laws and store rules change, and an independent developer cannot guarantee that every scenario is covered.

The developer does not receive cycle data through the app. For information voluntarily sent by email, the legal basis is described under User Rights.

International transfer: cycle databases are not transferred to developer servers. Email may be processed in jurisdictions where the mail providers operate (which may include countries outside the user's home country).

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

The app and this Privacy Policy are provided "as is" without warranties of any kind. Reasonable efforts are made to protect data and to describe practices accurately; uninterrupted service, accurate predictions, timely notifications, or absolute security cannot be guaranteed. Device security, backups, notification settings, PIN use, and content entered into the app remain the responsibility of the device owner.

The app may calculate, display, summarize, predict, or otherwise present cycle-related information based on data entered by the user. Such information may contain errors, omissions, inaccuracies, or limitations and should not be treated as a guarantee of accuracy. The developer is not responsible for decisions, actions, outcomes, or consequences resulting from reliance on information recorded, calculated, displayed, predicted, or notified by the app (including missed, delayed, or inaccurate period, fertility, ovulation, or pregnancy-related decisions).

To the maximum extent permitted by applicable law, Basic Organizer shall not be liable for indirect, incidental, special, consequential, or punitive damages, or for loss of data, arising from device failure, third-party services, missed or inaccurate notifications or predictions, reproductive or medical decisions, or circumstances beyond reasonable control. Total liability for claims relating to the app or this policy is limited to amounts paid for the app in the twelve months preceding the claim, or zero if the app was provided without charge, unless mandatory law prohibits such limitation. Some jurisdictions do not allow certain limitations; those provisions apply only to the extent permitted. Nothing in this policy limits rights or remedies that cannot be excluded under consumer or data-protection law.

---

## Privacy Policy Notice

This Privacy Policy is a notice of the app's privacy practices. It is not, by itself, a request for or a record of consent. Where applicable law requires consent for a particular processing activity (for example showing notifications or enabling backups), that consent is obtained through the relevant system or in-app control, not merely by reading this policy.

---

**Summary:**
- ✓ Cycle data stays on the device — the app does not declare internet permission and the developer does not operate servers for this app
- ✓ Cycle, health, and intimacy information is not transmitted **by the app** to Basic Organizer or to any server operated by Basic Organizer (user-enabled backups and voluntary emails are separate)
- ✓ No ads, analytics, advertising trackers, or accounts in the current version
- ✓ No AI or cloud services analyze health information; predictions run locally
- ✓ Google Backup and folder backup are optional; both in-app switches start off
- ✓ Folder backup files are readable JSON and may contain sensitive health / intimacy data — they should be kept somewhere trusted
- ✓ Optional local morning cycle notifications; not guaranteed; not for emergencies or contraception
- ✓ Optional app PIN stores a salted hash only; convenience lock, not a security guarantee
- ✓ Feedback emails include device model and Android version, and are sent only if the user sends them
- ✓ Cycle data can be edited, deleted, or copied (folder backup) in the app
- ✓ Not a medical device and not a contraceptive — informational personal tracking only
