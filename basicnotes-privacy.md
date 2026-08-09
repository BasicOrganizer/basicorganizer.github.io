# Privacy Policy for Basic Notes

**Last Updated: August 9, 2026**

## Introduction

This Privacy Policy explains how Basic Notes ("we", "our", or "the app") collects, uses, and protects information when you use our mobile application. We are committed to protecting your privacy and being transparent about our data practices.

## Developer Information

**App Name:** Basic Notes  
**Developer:** Basic Organizer  
**Contact Email:** basicorganizer.post@gmail.com

**Note:** This app is developed and maintained as an independent project. While we strive to provide reliable service and support, response times and feature development may vary based on available resources.

## Information We Collect

### Data Stored Locally

All user data is stored **locally on your device**:

- **Note Content:** Text content of your notes
- **Note Titles:** Titles of your notes
- **Timestamps:** Creation and last modified dates
- **Trash:** Notes moved to Trash are retained locally for up to 30 days before permanent deletion
- **App Preferences:** Settings, including language, sort order, theme (light/dark), and your backup choices (including the backup folder you selected)

This information is stored in a local SQLite database. By default it is **not** sent to the developer or to any server we operate.

### Optional backups

Backup is **optional**. Nothing is backed up by Basic Notes unless you enable a backup option in **Backup & Restore**. You can use either option, both, or neither.

**Google Backup**

- Only when you switch it on in the app *and* Google Backup is enabled in your phone settings.
- Your notes database and your backup settings are included in your device’s backup, which is uploaded to your own Google account.
- That backup is handled by Google under [Google’s Privacy Policy](https://policies.google.com/privacy), not by the Basic Notes developer. **We never receive, access, or host that data.**
- You can turn it off in the app at any time, and you can delete device backups in your Google account settings.
- Android and some device makers also offer their own backup and phone-to-phone transfer features. Basic Notes applies the same rule to those — it hands over nothing unless you have enabled Google Backup in the app — but those features are operated by your device manufacturer and by Google, not by us.

**Folder backup**

- Only when you switch it on and choose a folder using the system file picker (for example a folder on your phone, or in your own cloud storage).
- The app then writes a backup file to that folder about once a day, and keeps the **5 most recent** files, deleting older ones.
- The backup file is a **plain-text JSON file** containing your note titles, note content, creation and update times, starred marks, and notes still in Trash (with their deletion date). It is **not encrypted by the app**, so anyone who can open that folder can read your notes. Choose the folder accordingly.
- The file is written to the location *you* chose. **We never receive, access, or host those files.** If the folder is in a cloud service, that service’s own privacy policy and terms apply.
- Restoring from a backup **replaces** the notes currently in the app.
- You can turn folder backup off at any time, and you can delete the backup files yourself in that folder.

### Feedback emails

The app does not send anything to the developer on its own. If you use **Feedback**, the app opens *your* email app with a message prepared for you. To help with troubleshooting, that message is pre-filled with:

- Your device manufacturer and model
- Your Android version
- The Basic Notes version you are using

Nothing is sent unless you press send in your own email app, and you can edit or delete any of it first. When you do send it, we receive your email address, your message, and anything else you chose to include. We use it only to answer you and to fix problems, we do not use it for marketing, and we delete correspondence when it is no longer needed for that purpose.

### Permissions

Basic Notes does **not** request the Android **internet permission**, and it has no code to send your notes anywhere. Your notes cannot be uploaded to us.

The scheduling library used for folder backups (AndroidX WorkManager) adds these system permissions to the app, and they are used only to run the scheduled backup reliably:

- `WAKE_LOCK`, `FOREGROUND_SERVICE` — allow a backup already in progress to finish
- `RECEIVE_BOOT_COMPLETED` — restore the backup schedule after a restart
- `ACCESS_NETWORK_STATE` — used by the scheduler; the app does not access the network

Choosing a backup folder or exporting a file uses Android’s system file picker, which grants access only to the location you pick. The app does not request broad storage access.

### Third-Party Services

Currently, the app contains **no advertising, no analytics, no trackers, no crash-reporting service, and no user accounts**. The libraries it uses (AndroidX and Google Material components) provide user-interface and scheduling functions and do not collect your data.

Optional features **may** be introduced later:

- **Advertisements:** Device and usage information may be collected by third-party ad networks. Note content will **never** be shared.
- **Analytics:** Anonymous usage statistics may be collected to improve app performance.
- **Account-based cloud sync:** Optional synchronization that requires signing in. Requires explicit opt-in.
- **Cross-App Integration:** Optional sharing of data between authorized apps. Requires explicit consent.

All future features will be clearly disclosed in app updates or within the app interface, and users will have the option to **opt-in or opt-out**.

### Data We Do Not Collect

We operate no servers, and the app never transmits data to us by itself. We do not collect:

- Note content or titles
- Precise location data
- Contact lists
- Photos, media, or data from other apps
- Advertising identifiers or usage analytics

**One exception:** if *you* choose to email us (for example through **Feedback**), we necessarily receive your email address and whatever you write, as described above. We do not otherwise collect names, email addresses, or phone numbers.

---

## How We Use Your Information

- Notes and app data remain **local to your device**, unless you opt in to backup or use Share / Export.
- No note content is shared with the developer or used for advertising or analytics.
- When users use Share or Export, note content may be sent only to applications or file locations selected by the user; the developer does not collect or receive that data.
- When users opt in to Google Backup or folder backup, note data may be copied only as described above (Google’s backup systems, or a folder the user chooses).

---

## Data Security

- **Local Storage:** Notes are stored in a local SQLite database in the app’s private storage, which other apps cannot read.
- **No transmission by the app:** The app has no internet permission and does not upload your notes.
- **Optional backup:** Basic Notes only includes your notes in a backup after you enable Google Backup or folder backup in the app.
- **Backup files are not encrypted by the app:** A folder backup is a readable JSON file in the location you chose. Anyone with access to that folder or that cloud account can read it. Google Backup is protected by Google’s own systems and, on recent Android versions with a screen lock, is end-to-end encrypted by the device.
- **Device Security:** Data security also depends on your device’s own protections (screen lock, device encryption, who has access to the device).
- The app is provided by an independent developer and cannot guarantee absolute security.

---

## Children’s Privacy

- App is suitable for all ages.
- Does not knowingly collect personal information from children under 13.
- Any future ads will comply with child-safe standards and COPPA.

---

## Data Retention and Deletion

- Users can delete individual notes or all notes at any time.
- Notes in Trash are permanently deleted after 30 days unless restored or emptied sooner.
- Uninstalling the app removes local app data. **Backups you made are not removed by uninstalling:**
  - Folder backups stay in the folder you chose until you delete the files (the app keeps the 5 newest while folder backup is on).
  - Google Backup data stays in your Google account until you delete it in your device or Google account backup settings.
- The developer does not operate server-side note storage.
- Emails you send us are kept only as long as needed to handle your request, and can be deleted on request.

---

## User Rights

- Access, modify, delete, and export notes at any time.
- Opt in or out of optional backup features at any time in Backup & Restore.
- EEA/Norwegian users have rights under GDPR (access, rectification, erasure, portability, objection, complaint).

**Who is responsible (GDPR).** Because your notes stay on your device and we never receive them, we are not able to access, export, or delete them for you — you control them directly in the app. For the limited information you send us by email, the developer (Basic Organizer, contact below) acts as the data controller. The legal basis is our legitimate interest in answering your message and fixing problems in the app (GDPR Art. 6(1)(f)), or your consent where required.

**California (CCPA/CPRA).** We do not sell your personal information, and we do not share it for cross-context behavioural advertising. We do not use it to build profiles. California residents may exercise their rights by contacting us at the address below, and we will not discriminate against you for doing so.

### Right to Erasure ("Right to be Forgotten")
- You can delete individual notes or all notes within the app
- You can uninstall the app to remove local app data
- You can turn off backup and delete backup files or device backups you no longer want
- You can ask us to delete any email correspondence you have sent us
- Because we hold no notes or accounts, there is nothing else for us to delete on your behalf

---

## Changes to This Privacy Policy

- Updates will reflect the "Last Updated" date.
- Users will be informed of material changes via app updates or in-app notifications.
- Continued use of the app after changes constitutes acceptance.

---

## Legal Compliance

This policy is designed to comply with:

- **GDPR (EEA/Norway)**
- **CCPA (California, USA)**
- **COPPA (Children)**
- **Google Play Developer policies**

Optional features added in the future will also comply with applicable laws.

---

## Contact Us

**Email:** basicorganizer.post@gmail.com  
**Developer:** Basic Organizer

**Response Time:**
We will make reasonable efforts to respond to inquiries in a timely manner. For users in the European Economic Area (EEA), including Norway, we will respond to GDPR-related requests within 30 days as required by law, and may extend this period by an additional two months where necessary, taking into account the complexity and number of requests.

For other inquiries, we aim to respond as quickly as possible, but response times may vary.

When contacting us, please include:
- Your concern or request
- Your location (to ensure we apply the correct privacy laws)
- Any relevant details to help us assist you

---

## Disclaimer

This app is provided "as is" without warranties of any kind. While we make reasonable efforts to protect your data and comply with applicable privacy laws, we cannot guarantee uninterrupted service or absolute security. You are responsible for maintaining appropriate device security measures.

## Consent

By using Basic Notes, you consent to this Privacy Policy. If you do not agree, please do not use the app.

---

**Summary:**
- ✓ Notes stay on your device — the app has no internet permission and no servers behind it
- ✓ No note content is ever sent to the developer
- ✓ No ads, analytics, trackers, or accounts
- ✓ Google Backup and folder backup are optional — Basic Notes backs up your notes only after you enable one, and only to *your* Google account or *your* chosen folder
- ✓ Folder backup files are readable JSON — keep them somewhere you trust
- ✓ Feedback emails include your device model and Android version, and are only sent if you send them
- ✓ Users have full control over their data
- ✓ Written to align with GDPR, CCPA/CPRA, COPPA, and Google Play policies
