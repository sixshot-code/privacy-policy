---
layout: default
title: Privacy Policy for Lumina Library
---
# Privacy Policy for Lumina Library

**Effective date: 4 October 2026**

Lumina Library ("the App") is a reading tracker and library manager for books, series and audiobooks, with optional social features. It is available on iPhone, iPad, Apple Watch and Mac, and has a companion website, Lumina Web, that uses the same account.

The App is published by **Deon O'Brien, Dubai, United Arab Emirates**, referred to below as "we" or "I". For privacy purposes I am the data controller for the processing described here.

This policy describes what the App handles, what leaves your device, who receives it, and what we do not collect.

## Summary

- **Your library works on your device first.** Your books, reading progress, notes, quotes, tags, collections and tier lists are stored on your device, and sync privately between your own devices through your Apple Account if you enable iCloud. We cannot see that copy.
- **A guest identifier is created at launch.** The App starts an anonymous guest session with our backend, with a random identifier and no sign-in. It is used for the App's online services (subscription check, AI and search limits).
- **Signing in is optional.** If you sign in (with Apple or Google), your library is also stored on our backend so it can sync with Lumina Web, and so the optional social and shared-catalogue features work. Section 3 lists exactly what we hold.
- **Social features are opt-in and private by default.** A new profile is private, and publishing reviews, shelves or activity is off until you turn it on. Anything you choose to make public is visible to other readers.
- **We operate no analytics, crash-reporting or advertising SDKs**, and the App shows no advertising.
- **AI features are optional.** Some run on your device with Apple Intelligence. Others (Premium) send limited information to AI providers through our server. See section 5.
- **We never sell, rent or trade your information.**

## 1. Information on your device

Everything you add or create, including books, editions, formats, reading progress and sessions, ratings, notes, quotes, tags, collections, tier lists, preferences and challenges, is stored in the App's private database on your device. **Reading reminders and notifications are scheduled locally.** The camera is used only when you scan a book spine, cover or contents page, after you grant permission.

If you add a widget, Live Activity or Apple Watch app, the App shares the small amount of library information they show (such as a current book, its cover and progress) through storage private to the App on your devices.

## 2. iCloud sync

If iCloud is enabled on your device, the App's database also syncs through **Apple's CloudKit** into your own private iCloud container, governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/). **We have no access to it.** A few preferences sync through Apple's iCloud key-value store. You can turn this off in your device's iCloud settings.

## 3. Your account and what we hold on our servers

Our backend runs on **Supabase**. When you sign in, we hold the following against your account.

**Guest identifier.** The first time the App launches, it signs in to our backend **anonymously** and is issued a **random identifier (a UUID)**, before you use any feature and whether or not you ever sign in. It is not derived from your name, email, Apple Account, device identifier or any advertising identifier. It is used to check subscription status and to enforce fair-use limits on AI and book-search requests. Under UK and EU data-protection law it is nonetheless likely to count as **pseudonymous personal data**, and we treat it as such. You can delete a guest account in the App (Settings → Account).

**Account (if you sign in).** You can sign in with **Sign in with Apple** or **Google Sign-In**. We receive an identifier from that provider and the email address and name it chooses to share (Apple can give us a private relay address instead of your real one). We use these only to identify your account. We do not receive your Apple or Google password.

**Your library (when signed in).** To sync with Lumina Web and your devices, your library is stored in your account on our backend: your books and editions, reading progress and sessions, ratings and reviews you have written, notes and quotes, tags, collections, series and shelf placements, tier lists, audiobook bookmarks, reading challenges, followed authors and narrators, preferences, and recommendation feedback. This is private to your account unless you choose to publish it (see "Social features").

**Social features (optional).** If you set up a profile, we hold your **handle**, **display name**, **bio** and avatar choice, your visibility setting (private by default), and your choices about publishing reviews, shelves and activity. We also hold what you do in social features: follows and blocks, reviews and comments you post, shared lists and their members, buddy reads you create or join, notifications, **reports you make and moderation actions taken on accounts or content**, and your acceptance of the Community Guidelines. A **public** profile, and any review, shelf or activity you publish, can be seen by other readers.

**Shared catalogue.** Lumina keeps a curated reference catalogue of books, authors, series and editions. If you suggest a correction or submit information such as a narrator credit, we store the suggestion and who made it so it can be reviewed.

**Notifications.** If you allow push notifications (for example for new releases by authors you follow), we store a **device push token** and your follow list so we can send them. You can turn notifications off in the App or in iOS Settings.

**Purchases.** Lumina Premium is sold through Apple's In-App Purchase. Payment is handled entirely by Apple, and **we never see your payment details**. We use [RevenueCat](https://www.revenuecat.com/privacy/) to verify subscriptions: it receives your account identifier and the receipt Apple issues, plus standard device and app metadata, and returns whether Premium is active. We store whether Premium is active and when it expires.

**Usage limits.** We keep counters (such as how many AI or book-search requests an account has made in a period) to enforce fair-use limits and to keep costs under control.

## 4. Book search, covers and other requests

To find books and show covers, the App and our server make requests to book services. **The text you search for** (a title, author or ISBN) is sent to those services, some through our server and some from your device:

- **Open Library** and **Google Books** (searches, covers and metadata).
- **Apple's App Store/iTunes services** (audiobook and book covers and metadata from Apple's image servers).
- **Audnexus** (audiobook metadata).

Some links the App opens or recognises (such as retailer, Goodreads, StoryGraph or social-network links) go to those sites when **you** follow them, under their own policies. Any internet request reveals technical information such as your IP address, the time and the app name to whoever receives it. We do not use this to profile you.

If you share a link or book from another app into Lumina, the App reads that item on your device.

## 5. AI features

**On your device.** Where your device supports Apple Intelligence, some features can run on it and nothing leaves the device.

**Premium AI features (through our server).** Features such as Discover (taste-based recommendations), Mood Discovery, the Concierge chat, contents-scan cleanup and AI cover art are available to Premium users. When you use one, the App sends our server what the feature needs, **which can include information from your library** (for example titles, authors, ratings, tags, the reason you stopped reading a book, the books you are currently reading with your progress, and your reading queue) and **text you type** (a mood, a question to the Concierge, or text recognised from a contents-page scan). Our server forwards it to an AI provider and returns the result. Our server does not store the content of the request. We store a counter.

The providers currently used are **Google (Gemini)** and **DeepSeek**; DeepSeek is used as a fallback.

- **Google (Gemini API):** [privacy policy](https://policies.google.com/privacy) · [API terms](https://ai.google.dev/gemini-api/terms). Cover art generation uses Google's image model and sends your description.
- **DeepSeek (Open Platform API):** [privacy policy](https://cdn.deepseek.com/policies/en-US/deepseek-privacy-policy.html). DeepSeek's terms allow broader use than the other providers. **I cannot tell you that data sent to DeepSeek is never retained or never used for model development, and I do not claim that.** DeepSeek is based in China, so a request routed to it is processed there.

**Please do not enter information in an AI feature that you would not want a third party to retain.** Free features (for example short book blurbs and review summaries) use public book information, not your personal library. Our server also uses AI to help build the shared catalogue from public book information. That work does not use your personal data.

## 6. What we never collect

- Advertising or tracking identifiers, and no cross-app or cross-site tracking
- Your location
- Your contacts, photo library, calendar or health data
- Crash reports or analytics from third-party SDKs
- Your payment card or other payment details

## 7. How we use information

We use the information above only to provide the features you use (your library and sync, the social features you turn on, the shared catalogue, notifications, AI features, and verifying purchases), to enforce fair-use limits, and to keep the community safe and enforce the Community Guidelines (including acting on reports). We do not profile you for advertising and we do not use your information for marketing.

## 8. Retention and deletion

- **Your account and library** are kept while your account exists. **You can delete your account in the App** (Settings → Account). This permanently deletes your account on our backend, which removes your library and social data that is stored against it. The App then lets you choose whether to also keep or erase the copy stored on your device and in your iCloud.
- **Content you published** (reviews, comments, lists) is removed when you delete it or your account, except for copies other users legitimately made and records we must keep to run moderation and keep readers safe (such as a record that a report was made or an account was actioned).
- **Counters and usage limits** are kept only as long as needed to enforce limits.
- **Backups** held by our backend provider are overwritten on its normal schedule.
- **Retention by AI and other providers** follows their own terms, summarised in sections 4 and 5.

## 9. Your choices and your rights

- Keep your library on your device and in your own iCloud: **do not sign in**. (A guest identifier still exists, as described in section 3, but it is not linked to a name or email.)
- Keep your profile **private** (the default) and do not turn on publishing.
- **Block** or **report** other readers, and delete your own content.
- **Turn off notifications** in the App or in iOS Settings.
- **Delete your account** in the App.

If you are in the United Kingdom, the European Union, Australia, the United Arab Emirates or another region that grants data-protection rights (access, correction, erasure, portability, restriction or objection), you may exercise them by contacting us below. We will respond within the period the applicable law requires. Because most of your data is visible to you in the App, using the App's own controls is usually faster than a request to us.

Where a request involves information processed outside the country where you live (our backend and AI providers may process information in other countries, including the United States and China for DeepSeek), we rely on the safeguards the applicable law permits.

## 10. Security

We use reasonable technical and organisational safeguards, including encrypted transport, access controls and row-level security on our database, so that an account can read only its own private data. **No method of electronic storage or transmission is completely secure**, and we cannot guarantee absolute security.

## 11. Children

Lumina Library is not directed to children under 13, and the social features are not for anyone under 13. We do not knowingly collect personal information from children under 13. If you believe a child has an account, contact us and we will remove it.

## 12. Changes to this policy

If this policy changes materially, we will post the updated version at this URL with a new effective date before the change takes effect.

## 13. Contact

Questions about this policy, or a data-protection request:
**support@sixshot.app**

---
