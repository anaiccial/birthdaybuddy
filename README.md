# CakeBell Support

If you need help or have questions, please contact:

📧 Email: anaiccial@icloud.com

---

# Privacy Policy for CakeBell

**Last updated: September 1, 2026**

## Overview

CakeBell ("the App") is a birthday reminder application that helps you remember and celebrate your contacts' birthdays. This privacy policy explains how the App handles your data.

## How to Delete Your Data

CakeBell, developed by Markus Gaeth, lets you delete your server-side data directly in the App — no account or support request needed:

1. Open **CakeBell** on your phone
2. Go to the **Settings** tab
3. Scroll down and tap **"Delete my data"**
4. Confirm by tapping **"Delete"**

This immediately and permanently deletes your synced first names and birthdays, your reminder settings, and your device's push token from our database (see [What Data We Transmit](#what-data-we-transmit) below for exactly what that covers). Reminders are turned off until you re-enable them, which creates a fresh entry. **There is no additional retention period** — the database record is removed right away, not just deactivated.

If you've already uninstalled the App and still want your data deleted, email **anaiccial@icloud.com** with your approximate last-use date and device type (iOS/Android).

## Data Collection and Storage

### What Data We Access
- **Contact Information**: The App reads contact names and birthdays from your device's address book
- **Contact Photos**: Profile pictures from your contacts (if available) — these are never transmitted
- **User Preferences**: Your settings including reminder times, intervals, and relationship categorizations

### What Data We Transmit
To provide reliable birthday reminders via push notifications, the following minimal data is securely transmitted to our servers:
- **First names and birthday dates** (month and day only) of contacts with birthdays
- **Your reminder settings** (reminder time, interval, enabled/disabled)
- **Your device's push notification token** (assigned by Apple/Google, not personally identifiable)

### What Data We Do NOT Transmit
- No last names, phone numbers, email addresses, or photos
- No contact data of people without birthdays
- No message content or communication history
- No device identifiers, location data, or usage analytics

### How We Store Data
- **On your device**: All contact details, relationship types, and message preferences are stored locally using AsyncStorage
- **On our servers**: Only the minimal data listed above is stored in an encrypted AWS DynamoDB database in the EU (Frankfurt, Germany) to schedule push notifications

## Data Usage

We use the collected data solely to:
- Display upcoming birthdays
- Send push notifications for birthday reminders at your chosen time
- Generate personalized birthday messages (locally on your device)
- Organize contacts by relationship type

## Data Sharing

**We do not share, sell, or transmit your data to any third parties.**

Push notifications are delivered through Expo's push notification service, which acts as a relay to Apple Push Notification Service (APNs) and Google Firebase Cloud Messaging (FCM). No personal contact data is included in the push notification payload — only reminder text.

The App interacts with messaging applications (SMS, WhatsApp, Threema, Telegram) only when you explicitly choose to send a birthday message. These interactions are handled directly by the respective apps on your device.

## Permissions

The App requires the following permissions:
- **Contacts**: To read birthday information from your address book
- **Notifications**: To send birthday reminders via push notifications
- **SMS** (optional): To send text messages through your device's messaging app

## Data Retention

- Contact data is refreshed each time you open the App
- Server-side birthday data is overwritten with each sync and only reflects your current contacts
- Daily acknowledgment records (which birthdays you've already congratulated) are automatically reset every day
- User settings remain until you delete the App or request deletion via **Settings → Delete my data**
- Requesting deletion via the App removes your server-side record (names, birthdays, settings, push token) immediately and permanently
- Deleting the App removes all local data; without an explicit deletion request, server-side data becomes inactive (no more reminders are sent to a push token that no longer exists) but is not automatically purged

## Data Security

- Local data is protected by your device's security measures (passcode, biometric authentication, etc.)
- Server-side data is stored in AWS DynamoDB with encryption at rest in the EU (Frankfurt)
- All communication between the App and our servers uses HTTPS/TLS encryption
- Our backend infrastructure runs on AWS Lambda with no persistent servers, minimizing attack surface

## Your Rights

You can:
- Revoke permissions at any time through your device settings
- Request deletion of your server-side data (synced names and birthdays, reminder settings, push token) at any time via **Settings → Delete my data** inside the App. This immediately and permanently removes your entry from our database; reminders are turned off until you re-enable them, which starts a fresh sync
- Delete all App data, including local data on your device, by uninstalling the application
- Modify relationship types and messaging preferences within the App

## Children's Privacy

The App does not knowingly collect data from children under 13. The App is designed for general audiences.

## Changes to This Policy

We may update this privacy policy from time to time. Changes will be reflected in the "Last updated" date above.

## Contact

For questions about this privacy policy, please contact:
anaiccial@icloud.com

## Compliance

This App complies with:
- Apple App Store Guidelines
- Google Play Store Guidelines
- General Data Protection Regulation (GDPR) — data is stored in the EU (Frankfurt, Germany)
- California Consumer Privacy Act (CCPA) principles
