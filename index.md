# Privacy Policy for Pocketly

**Last updated: November 11, 2026**

Pocketly ("Pocketly", "we", "our", or "the app") is a personal finance tracking application designed with an offline-first approach. This Privacy Policy explains what data Pocketly handles, how it is stored, and what control you have over your data.

## 1. Data Collection and Storage

### Local Storage Only

Pocketly is designed to operate locally on your device. Your financial information, including transactions, income, expenses, investments, budgets, categories, staged SMS review entries, learned merchant category rules, and app settings, is stored strictly on your device using an on-device SQLite database (Room) and Android Preferences DataStore.

### No Cloud Storage or User Accounts

Pocketly does not require you to create an account and does not maintain a cloud database or user account system.

Your financial records and SMS data are never uploaded to Pocketly's servers or synchronized to a Pocketly cloud service.

### No Analytics, Ad Tracking, or Data Selling

Pocketly does not use third-party advertising SDKs, behavioral analytics SDKs, tracking pixels, or marketing trackers to monitor your activity within the app.

We never sell, rent, share, or transfer your financial activity or SMS data to advertisers, data brokers, or third parties.

## 2. Internet and Third-Party Services

Pocketly's core financial tracking and on-device SMS parsing functionality work completely offline without requiring an Internet connection.

Pocketly does not transmit your financial records or text messages to a Pocketly-operated or third-party remote server.

If a future version of Pocketly introduces an online or third-party service that processes personal data, this Privacy Policy will be updated before or when that functionality is introduced, as applicable.

## 3. Permissions and Device Access

Pocketly requests only permissions needed to provide specific local features. Optional permissions require explicit user consent and are preceded by an in-app disclosure explaining how they are used.

### SMS Messages (Optional — SMS-Based Money Management)

**READ_SMS and RECEIVE_SMS:**

When you explicitly opt in to **Auto-Read SMS** or run **Scan Current Month Now** in Settings, Pocketly requests `READ_SMS` and `RECEIVE_SMS` permissions after presenting an in-app **"On-Device SMS Detection"** disclosure dialog.

- **Purpose:** Strictly used as an on-device personal money management feature to detect financial transaction alerts (such as bank, card, or payment debit/credit messages) and stage them for your review before logging them into your ledger.
- **Scope & Filtering:** Initial inbox scanning reads only messages from day 1 of the current calendar month onward. Non-transactional SMS—including OTPs, PINs, CVVs, promotional messages, and failed alerts—are ignored in memory and never stored.
- **User Control & Retention:** Recognized transactions are staged locally in the **Pending** queue in **SMS Inbox** until you review, edit, approve, or ignore them. Once a staged item is approved or ignored, the raw SMS message body is cleared (`null`) from local database storage. User-learned merchant-to-category mappings are stored locally to improve future categorization and can be edited or deleted anytime in **SMS Inbox → Learned Rules**.
- **Strict Limited Use:** All SMS parsing runs 100% locally on your device. Zero SMS content leaves your device or is used for advertising, profiling, or non-core purposes.

### Notifications

**POST_NOTIFICATIONS (Android 13 and later):**

Used to provide local notifications when enabled by you, including daily expense logging reminders and optional alerts when a new transactional SMS is staged in your Inbox queue for review.

Notifications can be disabled anytime through Pocketly Settings or your Android device settings.

### Device Reboot

**RECEIVE_BOOT_COMPLETED:**

Used to restore locally scheduled expense reminder alarms after your device restarts.

This permission does not give Pocketly access to your financial records or SMS outside the app's local storage.

### File Import and Export

When you explicitly choose to export, import, or create a backup of your data, Pocketly uses Android's system file picker to allow you to select a file.

Pocketly accesses only the files that you explicitly select for import, export, or backup restore.

## 4. Data Export and Portability

Pocketly gives you control over your financial data.

Through the **Data & Support** section in Settings, you can export supported financial data in CSV or JSON format, or generate full local backup snapshots (including transactions, categories, budgets, staged SMS entries, and learned merchant rules).

Exported and backup files are stored in the location you choose. Once exported, those files are under your control, including if you choose to store them on a personal cloud storage service or other storage location.

Pocketly does not control or have access to copies of files that you independently store outside the app.

## 5. Data Retention and Deletion

Because Pocketly stores financial data locally on your device, the data remains there until you remove it or clear the app's data.

### Delete Account & Data

Pocketly provides a **Delete Account & Data** option in Settings. Because Pocketly does not maintain a cloud account, this function permanently deletes all locally stored Pocketly data (transactions, budgets, categories, staged SMS items, learned merchant rules, and preferences) and resets the app on your device.

You should export any data you want to keep before using this option.

### Uninstalling the App

Uninstalling Pocketly removes the app's locally stored application database and preferences from your device in accordance with Android's app-data handling. Any exported CSV/JSON files or backups that you previously saved outside the app are not automatically deleted by Pocketly.

## 6. Security

Pocketly's offline-first architecture ensures your financial records and parsed SMS alerts remain strictly on your device rather than being transmitted to remote servers.

You are responsible for maintaining the security of your device, including using appropriate device-level protections such as a screen lock, OS updates, or device encryption.

No method of electronic storage can be guaranteed to be completely secure.

## 7. Children's Privacy

Pocketly is a general-audience personal finance utility.

Pocketly does not knowingly collect personal information from children or from users generally through a remote data-collection system.

If you believe that personal information has been provided to us in a manner that should not have occurred, please contact us using the information below.

## 8. Changes to This Privacy Policy

We may update this Privacy Policy when Pocketly's features, data practices, or applicable requirements change.

When we make changes, we will update the **Last updated** date at the top of this policy. We encourage you to review this page periodically.

## 9. Contact

If you have questions about this Privacy Policy, Pocketly's data practices, or the handling of your data, you can contact us by email:

**Email:** abvibelabs@gmail.com

---

**Pocketly**  
Offline-first personal finance tracking.
