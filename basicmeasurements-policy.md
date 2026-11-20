# Privacy Policy for Basic Measurements

**Last Updated: November 20, 2026**

## Introduction

This Privacy Policy explains how Basic Measurements ("we", "our", or "the app") handles information in connection with the Android mobile application (package name: `com.basicorganizer.measurements`).

**Basic Measurements stores information you enter locally on your device. The developer does not receive or have access to that information through the app.** Optional backups, optional export, optional reminders, and voluntary emails are described separately below.

This policy covers the Basic Measurements Android application published by Basic Organizer. It does not govern Google Play, email providers, Google's backup systems, device manufacturers, or other third-party services. Those parties have their own policies.

Basic Organizer develops and maintains the app as an independent project. The application does not operate developer-run servers. Weight, body measurements, personalization details, or other content you enter is **not transmitted by the app** to Basic Organizer or to any server operated by Basic Organizer. This document is provided for transparency and does not constitute legal advice.

## Developer Information

**App Name:** Basic Measurements (device label: Measurements)  
**Developer:** Basic Organizer  
**Contact Email:** basicorganizer.post@gmail.com  
**Distribution:** Google Play Store

**Note:** This app is developed and maintained as an independent project. While we strive to provide reliable service and support, response times and feature development may vary based on available resources.

---

## Not Medical Advice; Informational Tracking Only

Basic Measurements is a personal tool for logging body weight and body measurements, viewing on-device statistics (including BMI and waist-to-hip ratio), and optionally setting reminders. It is **not a medical device**, healthcare service, diagnostic tool, treatment tool, or clinical monitoring service, and it does **not** provide medical, fitness, nutritional, or professional advice.

**Do not rely on this app for medical diagnosis, treatment decisions, urgent care, emergency situations, or any other health-related decision that requires a qualified professional.**

Calculated values such as BMI and waist-to-hip ratio, and statistics, graphs, trends, category labels, and similar summaries, are automatically generated estimates based only on the information you enter and on simple local algorithms. They may be incomplete, inaccurate, or unsuitable for decision-making — especially with incomplete logging, atypical body composition, pregnancy, illness, or other factors. They do **not** fully reflect muscle mass, fat distribution, or overall health.

Users should not rely on the app as their only means of remembering weigh-ins, measurements, appointments, medications, or other time-sensitive matters. If you have concerns about your health, weight, or body composition, consult an appropriately qualified healthcare professional.

The app is not intended to replace professional advice, diagnosis, treatment, or emergency services.

This app is not provided as part of a HIPAA-covered healthcare service, and this Privacy Policy is not a HIPAA Notice of Privacy Practices.

---

## Health and Sensitive Information

Information you enter into Basic Measurements — including body weight, body circumferences, height, date of birth, sex, and derived values such as BMI or waist-to-hip ratio — may be considered **sensitive personal information** or health-related information under certain laws (including special-category data under GDPR / UK GDPR where applicable).

This information is stored **locally on your device** by default and is **not transmitted by the app** to Basic Organizer or to any server operated by Basic Organizer. Optional backup and export features can create copies outside the app's private storage, as described below. Optional reminders may display measurement-related text on the device notification shade when enabled and permitted by the system.

The app uses this information locally to provide logging, on-device calculations and charts, personalization, optional reminders, optional export, and related functionality. It may also be included in optional backups enabled by the user, in export files the user creates, or in communications the user voluntarily sends to the developer. **Basic Organizer does not use this information for advertising, profiling, analytics, or marketing**, and does not sell it or share it with third parties for those purposes.

Basic Measurements does **not** use artificial intelligence or external cloud services to analyze your measurement data. Calculations and statistics run **locally on your device**.

Users are responsible for the information they choose to enter, including whether it is appropriate to store on their device or in any backup or export location. Users should not use the app to store information that they are legally prohibited from storing, information belonging to another person without appropriate authorization, passwords, authentication credentials, financial credentials, or other information requiring a level of security that the app does not provide.

---

## No Emergency or Safety-Critical Use

Basic Measurements is not designed or intended for emergency communications, emergency notifications, safety monitoring, crisis detection, medical-alarm delivery, or other safety-critical purposes. Optional reminders should not be relied upon to identify emergencies or to notify others when assistance may be required.

---

## Information Stored in the App

In this policy, "stored" means information kept in the app's local storage on the device for the app to function. That is **not** the same as information being received, accessed, or collected by Basic Organizer. Unless this policy expressly says otherwise (for example optional backups, export, or a voluntary email), Basic Organizer does not receive that information.

### Data Stored Locally

Application data required for ordinary operation is stored **locally on the device**:

- **Weight entries:** Body-weight values you enter, with dates and (for same-day entries) optional times
- **Body measurements:** Circumference values you enter for waist, hips, chest/bust, upper arm, and thigh, with dates
- **Personalization (optional):** Sex, date of birth, and height, used on-device for features such as BMI estimates and age-aware category labels where applicable
- **Reminder preferences:** Whether reminders are enabled, and the frequency (daily or weekly), time, and weekday you choose
- **App preferences:** Language (including system default); theme (light / dark / system); units (metric / imperial); date and time formats; and backup choices (including the backup folder selected, if any)

This information is stored in a local SQLite database and in app-private SharedPreferences. The app does **not** transmit it to Basic Organizer or to any server operated by Basic Organizer. Optional backup and export features can create copies of some of this data outside the device, as described below.

### Optional reminders

Reminders to note measurements are **optional**. They can be turned on or off in **Reminders**. When enabled and the system allows notifications, the app may schedule a **local** daily or weekly reminder at the time you choose.

Reminder text may include wording about logging weight or body measurements. **Notification content is not transmitted by the app to Basic Organizer or to any server operated by Basic Organizer.**

On Android 13 and later, the app declares the **POST_NOTIFICATIONS** permission. Saving reminder settings may prompt for that permission where required. If permission is denied, or if notifications are blocked in system settings, reminders may not appear even though the in-app reminder switch remains on.

Where required by Android, the app may also use exact-alarm scheduling so reminders can fire closer to the time you chose. Exact-alarm capability depends on system settings and may be restricted by the device.

After a device restart or app update, the app may reschedule the next reminder locally. Delivery can be affected by Do Not Disturb, battery optimization, Doze mode, manufacturer-specific power management, timezone changes, or other system settings outside the developer's control. **Reminders are not guaranteed to fire at the exact intended moment, or at all.**

Tapping a reminder opens the app. The current version is not designed to send notification events to advertising, analytics, or crash-reporting services.

### Optional backups

Backup is **optional**. In the app, both Google Backup and folder backup are **off by default** until switched on in **Backup & Restore**. Either option, both, or neither may be used.

Because measurement data may include sensitive health-related information, users should consider carefully whether to enable backups and where folder backup files are stored.

**Google Backup**

- The app allows Android backup (`allowBackup`). A custom full-backup agent is designed to include the measurements database and related backup-preference files only when the in-app Google Backup option is switched on; if that option is off, the agent is designed to back up nothing through that cloud-backup path. (Key/value backup APIs are unused.)
- Measurement data is added to Google Backup only when the Google Backup option is switched on in **Backup & Restore** *and* Google Backup is enabled in device settings. When included, that backup **may contain**:
  - The measurements SQLite database (weight entries and body-measurement entries)
  - Backup preference settings (such as opt-in flags and, if folder backup was configured, the chosen folder location)
- Personalization and other general app preferences (for example height, date of birth, sex, theme, language, units, date/time formats, and reminder schedule) are **not** currently included in the Google Backup path described above. They remain in local app preferences on the device unless you re-enter them after reinstall.
- That backup is handled by Google under [Google's Privacy Policy](https://policies.google.com/privacy), not by the Basic Measurements developer. **The developer does not receive, access, or host that data.** Google operates and controls its backup service, including its applicable security, retention, restoration, and deletion mechanisms. Those practices are governed by Google's applicable policies and settings. **Basic Organizer does not control those mechanisms.**
- The option may be turned off in the app at any time. Turning it off stops the app from adding measurement data to later backups that use the Android cloud backup system. Copies already stored by Google remain until deleted in Google account or device backup settings.

**Device transfer and manufacturer tools**

- The app's Google Backup switch is designed to control what the app includes in **cloud** backups that use the Android backup agent described above. It does **not** necessarily control every Android or manufacturer copy, transfer, cloning, or migration path.
- Android device-to-device transfer and similar manufacturer tools may copy application data according to the app's declared data-extraction rules and according to the manufacturer's own settings and policies. Those paths can include the measurements database and related backup-preference files even when the in-app Google Backup switch is off.
- The developer does not control third-party device backup, migration, cloning, synchronization, restoration, or transfer mechanisms. Such mechanisms may copy, retain, modify, omit, or otherwise process application data independently of the app's own backup settings.

**Folder backup**

- Only when switched on and a folder is chosen with the system file picker (for example a folder on the device, or in the user's own cloud storage).
- When folder backup is enabled, a backup file is written promptly, then about once a day (the schedule may be delayed if the battery is low). The app attempts to keep the **5 most recent** backup files it created in that folder and may delete older backup files it created when a new one is written.
- The backup file is a **plain-text JSON file** containing weight entries and body-measurement entries, plus backup metadata (such as format version, app label, and export time). **Personalization and other app preferences are not currently included in the folder backup JSON.** The folder backup file is **not encrypted by the app**. Anyone with access to that folder can read its contents, which may include sensitive health-related information. The folder should be chosen accordingly.
- Files are written only to the location chosen by the user. **The developer does not receive, access, or host those files.** If the folder is in a cloud service, that service's own privacy policy and terms apply.
- Restoring from a backup **replaces** the weight and body-measurement data currently in the app.
- Folder backup may be turned off at any time. Turning it off stops further automatic writes. Existing backup files remain in the folder until the user deletes them.

**User responsibility for backups**

Users are responsible for deciding whether to enable backups and where folder backup files are stored. Because folder backup files are not encrypted by the app and may contain sensitive health-related information, users should choose a storage location they consider appropriate. The developer does not control third-party storage locations (including cloud folders) and cannot guarantee their security or availability. **The developer cannot control or verify the security, privacy, availability, retention, deletion, or backup practices of any storage provider or location selected by the user.** Nothing in this section limits rights or remedies that cannot be excluded under applicable law.

### Optional export created by you

You may choose to **export** your weight and body-measurement entries to a text file (optionally including a statistics summary). That file is created **only when you request it**. The app then opens your device's system share sheet so **you** can save or send the file using apps or locations you choose.

If you include statistics, the export may also contain derived values such as weight ranges, BMI estimates (when height is set), and waist-to-hip ratio. A temporary copy of the export file may be created in the app's private cache so the system share sheet can open it.

Once you export a file, that copy is under **your** control. **Once exported, files are no longer protected by the app and are subject to the security of the location where they are stored.** Exported files may contain sensitive health-related information. The app does not upload exports to the developer. If you store or share an exported file outside the app (for example in cloud storage, messaging, or email), that is outside the app's control and subject to the policies of those services or recipients.

### Feedback emails

The app does not send messages to the developer on its own. If **Feedback** is used, the device email application is opened with a message prepared for the user. To assist troubleshooting, that message is pre-filled with:

- Device manufacturer and model
- Android version (SDK level)
- The Basic Measurements version in use (in the email subject)

Nothing is sent unless the message is sent from the user's own email application. The contents may be edited or deleted first. When a message is sent, the developer receives the sender's email address, the message, and anything else included (which may include measurement or health content if the sender pastes it). Correspondence is used only to respond to the request and to resolve related issues, is not used for marketing, and is retained only for as long as reasonably necessary for those purposes. Deletion of correspondence may be requested using the contact details below. Email is delivered through the sender's and the developer's mail providers, which have their own policies.

### Permissions

The app declares the following permissions. None of them are used by the app to transmit measurement content to Basic Organizer or to any server operated by Basic Organizer.

- **POST_NOTIFICATIONS (Android 13+):** Used to display optional local measurement reminders when the user has enabled reminders and system notification permission is granted.
- **SCHEDULE_EXACT_ALARM:** Used to deliver reminders closer to the times you choose, where required and allowed by Android.
- **RECEIVE_BOOT_COMPLETED:** Used to reschedule the next local reminder after the device restarts or the app is updated.
- **VIBRATE:** Used for optional notification feedback where supported by the device.

**The app does not transmit measurement data to Basic Organizer or to a developer-operated server.** The app's application code is designed not to upload measurement data to Basic Organizer or a developer-operated server. As supporting evidence of that design, the app does **not** declare the Android **INTERNET** permission.

AndroidX WorkManager and other bundled Android components may contribute system permissions required for background scheduling (for example for folder backup). Some of these permissions can include `WAKE_LOCK`, `FOREGROUND_SERVICE`, or `ACCESS_NETWORK_STATE`. Their presence does not mean that Basic Measurements uploads measurement data to the developer or to a developer-operated server. Folder backup scheduling is handled by WorkManager and may continue after reboot according to Android's background-work behavior; the app may also re-schedule folder backup when opened if that option is still enabled.

Choosing a backup folder or exporting a file uses Android's system file picker / share sheet, which grants access only to the location selected. The app does not request broad storage access. Opening an external link (for example the developer page on Google Play via **More apps**) uses the system to launch another application; it does not grant this app network access for uploading measurement data.

### Third-Party Services

The current version of the app contains **no advertising, no analytics, no advertising trackers, no crash-reporting service, and no user accounts**. The libraries it uses (AndroidX and Google Material components) provide user-interface and scheduling functions. They are not used by the developer to collect user data.

If this ever changes, this policy and the app's Data safety information on Google Play will be updated before the change is released, and consent will be requested where the law requires it.

The following user-initiated actions involve third parties not controlled by Basic Organizer:

- **Feedback:** Opens the device's email application as described above. Transmission of any message is governed by the email providers' policies.
- **Export share sheet:** Opens apps or locations you choose. Those parties process the exported file under their own policies.
- **More apps / developer page on Google Play:** Opens Google Play or a browser. Data processing by Google is governed by [Google's Privacy Policy](https://policies.google.com/privacy).
- **Google Play distribution:** Installation, updates, ratings, and store interactions involve processing by Google as store operator.
- **Optional Google Backup:** If enabled, device backup that uses the Android cloud backup system is processed by Google as described above.
- **Device transfer / manufacturer tools:** May process app data as described under Device transfer and manufacturer tools above.

### Information the Developer Does Not Receive Through the App

The developer does not operate servers for this app. Through ordinary use of the app, the following are **not transmitted by the app** to Basic Organizer or to any server operated by Basic Organizer:

- Weight entries, body measurements, height, date of birth, sex, BMI estimates, waist-to-hip ratio estimates, or other health-related entries
- Statistics, charts, reminder text, or export content
- Precise location data
- Contact lists
- Photos, media, or data from other apps
- Advertising identifiers or usage analytics

Google Play, Google Backup, email providers, Android, and device manufacturers may process information in connection with their respective services under their own policies. The developer does not control those services.

**User-initiated email is different:** if the user chooses to email the developer (for example through **Feedback**), the developer necessarily receives the email address and whatever is written, as described above. Names, email addresses, and telephone numbers are not otherwise received by the developer through the app.

---

## How We Use Your Information

- Measurement data and application preferences remain **local to the device**, unless a backup, export, or device-transfer path is used as described above.
- Measurement content is not used for advertising or analytics, and is not transmitted **by the app** to Basic Organizer or to any server operated by Basic Organizer, except if the user includes it in an email.
- When Google Backup or folder backup is enabled, measurement data may be copied as described above. Separate manufacturer transfer tools are described in the backup section.
- When reminders are enabled and system permission allows it, reminder scheduling and notifications occur locally on the device.
- Voluntary email is used only to respond to support inquiries and to resolve related issues.
- Personal information is **not sold**. Personal information is **not shared** for cross-context behavioral advertising.

---

## Data Security

- **Local Storage:** Measurement data is stored in a local SQLite database and app-private preferences. Other apps cannot read that storage in ordinary Android use. They may be readable on a rooted or compromised device, or by someone with physical access to an unlocked device.
- **No upload by the app:** The app's application code is designed not to upload weight, body-measurement, or personalization content to Basic Organizer or a developer-operated server. As supporting evidence of that design, the app does not declare the Android INTERNET permission.
- **Optional backup:** Measurement data is added to Google cloud backup (via the Android backup agent) or written as a folder backup only after the corresponding option is enabled in the app. Device-transfer paths are described separately above.
- **Backup files are not encrypted by the app:** A folder backup is a readable JSON file in the chosen location. Anyone with access to that folder or that cloud account can read it, including sensitive health-related information if present. Google Backup is handled by Google under Google's own systems and policies. The developer does not control those systems.
- **Reminders:** Reminder scheduling and notifications are processed locally. Their reliability depends on device settings and system behavior.
- **Device Security:** Data security also depends on the device's own protections (screen lock, device encryption, and who has access to the device).
- The app is provided by an independent developer and cannot guarantee absolute security.

---

## Data Preservation

The developer does not guarantee that measurement data will remain available indefinitely. Data may be lost or become inaccessible due to device failure, operating-system changes, application errors, accidental deletion, uninstallation, storage failure, backup failure, restoration of an earlier backup, device replacement, missed or blocked reminders, or other circumstances outside the developer's control.

Users are responsible for enabling and maintaining backups if they require copies of their data.

---

## Children's Privacy

- Basic Measurements is intended for people who wish to track personal body measurements. The app is **not directed at children** and is not marketed to children.
- The app is not age-restricted or age-gated. It contains no advertising and no features designed to appeal specifically to children.
- Measurement data stays on the device and is not transmitted **by the app** to Basic Organizer or to any server operated by Basic Organizer through ordinary use of the app. The only way information can reach the developer is if someone chooses to send an email.
- The developer does not knowingly collect personal information from children in circumstances where applicable law requires parental consent or otherwise restricts such collection. If it is believed that a child has sent personal information by email, contact the address below and it will be deleted.

---

## Data Retention and Deletion

- Individual weight entries and body-measurement entries may be deleted within the application at any time.
- Personalization and reminder settings may be changed or cleared within the application at any time.
- Uninstallation of the application removes locally stored app data under standard Android behavior. **Backups and exports already made are not removed by uninstalling:**
  - Folder backups remain in the chosen folder until the files are deleted (while folder backup is on, the app attempts to keep the 5 newest backup files it created).
  - Google Backup data remains in the Google account until deleted in device or Google account backup settings.
  - Exported files previously saved or shared outside the app remain until the user deletes them.
- The developer does not operate server-side measurement storage.
- Feedback correspondence is retained only for as long as reasonably necessary to respond to the request and resolve related issues. Deletion of correspondence may be requested using the contact details below.

---

## User Rights

- Access, modify, and delete measurement data through the application.
- Copy measurement data by using folder backup (JSON) or the in-app export feature (text file).
- Opt in or out of optional backup features at any time in Backup & Restore.
- Enable or disable reminders in Reminders, and control notification permission and alarm-related settings in system settings.
- Users in the EEA and United Kingdom may have rights under GDPR / UK GDPR (access, rectification, erasure, portability, objection, complaint to a supervisory authority), including rights relating to special-category / health data where applicable.

**Who is responsible (GDPR / UK GDPR).** Measurement data stays on the device and is not received by the developer through the app, so the developer cannot access, export, or delete measurement data on the user's behalf — that control is exercised directly in the app. Requests concerning locally stored measurement data can generally be fulfilled directly by deleting the data within the app or removing the app, rather than by contacting the developer. For information voluntarily provided by email, the independent developer who publishes this app under the name Basic Organizer (contact below) acts as the data controller and processes that information only as necessary to respond to the inquiry and manage related support. The applicable legal basis under Article 6 GDPR / the corresponding UK GDPR requirements depends on the circumstances. Where the information includes special-category personal data, processing will additionally rely on an applicable condition under Article 9 GDPR / the corresponding UK GDPR requirements where required (this Privacy Policy is not itself consent; see Privacy Policy Notice below).

**California (CCPA/CPRA).** To the extent the California Consumer Privacy Act, as amended, applies to Basic Organizer, personal information is not sold and is not shared for cross-context behavioral advertising, and is not used to build profiles. California residents may exercise applicable rights by contacting the address below. There is no discrimination for doing so. The categories of sensitive personal information that may be stored locally by the app, and the circumstances in which information may leave the device through user-enabled backups, exports, device transfer, or voluntary communications, are described in this policy.

Privacy requests: **basicorganizer.post@gmail.com** (subject: "Privacy request - Basic Measurements"), including the nature of the request, jurisdiction, and relevant particulars. GDPR-related requests will be answered within one month where required, with extension by up to two further months where permitted for complex cases.

### Right to Erasure ("Right to be Forgotten")

- Individual weight or body-measurement entries may be deleted within the application
- The application may be uninstalled to remove local app data
- Backup may be turned off, and backup files, device backups, or exports that are no longer wanted may be deleted
- The developer may be asked to delete any email correspondence that has been sent
- Because the developer does not hold measurement data or user accounts, there is no developer-held measurement database to delete. Requests concerning locally stored measurement data can generally be fulfilled directly by deleting the data within the app or removing the app. Any personal information contained in support correspondence can be handled as described in the Feedback emails and Data Retention sections.

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

The developer does not receive measurement data through the app. For information voluntarily sent by email, the applicable legal basis is determined as described under User Rights.

International transfer: measurement databases are not transferred to developer servers. Email may be processed in jurisdictions where the mail providers operate (which may include countries outside the user's home country).

---

## Contact Us

**Email:** basicorganizer.post@gmail.com  
**Published under the name:** Basic Organizer

**Response Time:**
Reasonable efforts will be made to respond to inquiries in a timely manner. For users in the European Economic Area (EEA) and the United Kingdom, GDPR-related requests will be answered within one month as required by law, and may be extended by up to two further months where necessary, taking into account the complexity and number of requests.

For other inquiries, responses will be provided as promptly as practicable; timing may vary.

When contacting us, please include:
- The concern or request
- Location (jurisdiction), to apply appropriate privacy law
- Relevant details to facilitate handling

---

## Disclaimer

The app and this Privacy Policy are provided "as is" without warranties of any kind. Reasonable efforts are made to protect data and to describe practices accurately; uninterrupted service, accurate calculations, timely reminders, or absolute security cannot be guaranteed. Device security, backups, exports, notification settings, and content entered into the app remain the responsibility of the device owner.

The app may calculate, display, summarize, or otherwise present measurement-related information based on data entered by the user. Such information may contain errors, omissions, inaccuracies, or limitations and should not be treated as a guarantee of accuracy. **Do not rely on BMI, waist-to-hip ratio, charts, or trends as medical advice.** The developer is not responsible for decisions, actions, outcomes, or consequences resulting from reliance on information recorded, calculated, displayed, or notified by the app (including missed, delayed, or inaccurate reminders or estimates).

To the maximum extent permitted by applicable law, the developer shall not be liable for any direct, indirect, incidental, consequential, or special damages arising from the use of, inability to use, or reliance upon the app or its features, including medical or fitness decisions, inaccurate estimates or statistics, missed reminders, data loss, device failure, or use of exported or backup files after they leave the app. Some jurisdictions do not allow certain limitations of liability; in those places, liability is limited to the fullest extent permitted by law.

---

## Privacy Policy Notice

This Privacy Policy is a notice of the app's privacy practices. It is not, by itself, a request for or a record of consent. Where applicable law requires consent for a particular processing activity (for example showing notifications or enabling backups), that consent is obtained through the relevant system or in-app control, not merely by reading this policy.

---

**Summary:**
- ✓ Measurement data stays on the device — the app does not declare internet permission and the developer does not operate servers for this app
- ✓ Weight, body measurements, and personalization are not transmitted by the app to Basic Organizer or a developer-operated server; user-enabled backups, exports, and voluntary emails are separate
- ✓ No ads, analytics, advertising trackers, or accounts in the current version
- ✓ No AI or cloud services analyze health information; calculations run locally
- ✓ Google Backup and folder backup are optional; both in-app switches start off
- ✓ Folder backup files are readable JSON (weight and body measurements) — keep them somewhere trusted
- ✓ Restore from folder backup replaces the measurement data currently in the app
- ✓ Phone-to-phone / manufacturer transfer may copy app data under system rules, separately from the Google Backup switch
- ✓ Optional local measurement reminders; not guaranteed; not for emergencies
- ✓ Optional export is user-initiated; once exported, files are no longer protected by the app
- ✓ Feedback emails include device model and Android version, and are sent only if the user sends them

- ✓ Measurement data can be edited, deleted, or copied (folder backup / export) in the app
- ✓ Not a medical device — BMI and similar values are informational mathematical estimates only
