---
layout: default
title: Privacy Policy for Expired
---
# Privacy Policy for Expired

**Effective date: 4 October 2026**

Expired ("the App") helps you track subscriptions, memberships and documents, and reminds
you before they renew or expire.

The App is published by **Deon O'Brien, Dubai, United Arab Emirates**, referred to below as "we" or "I". For privacy purposes I am the data controller
for the limited processing described here.

This policy describes exactly what the App handles, what leaves your device, and what we
never collect.

## Summary

- **No account is required.** There is no sign-up. We never ask for your name, email
  address or password.
- **Your item data stays on your device**, and — if you enable iCloud — syncs privately
  between your own devices through your Apple Account. We cannot see it.
- **We operate no analytics, crash-reporting or advertising SDKs**, and we show no
  advertising.
- We hold three small server-side records about you: a random identifier, a daily
  **count** of AI requests, and whether your Pro subscription is active. Details below.
- By default the App also reports **which well-known services** (for example "Netflix")
  are tracked on your device, as an anonymous tally with no identifier stored against it.
  You can turn this off in Settings → Privacy & Security. See section 5.
- **We never sell, rent or trade your information.**

## 1. Information stored on your device

Everything you enter — item names, costs, billing cycles, renewal and expiry dates,
categories, notes, website addresses, and any account email, username or password you
choose to record against an item — is stored locally on your device in the App's private
database. When you change an item's price, the App also keeps the **previous price and the
dates it applied**, so its spending recap stays accurate; this is item data like the rest.

**Reminders are scheduled and delivered locally by your device.** We operate no
push-notification server, and no reminder passes through us.

## 2. iCloud sync

If iCloud is enabled on your device, the App's database also syncs through **Apple's
CloudKit** into your own private iCloud container, so your items appear on your other
devices. That container belongs to your Apple Account and is governed by
[Apple's Privacy Policy](https://www.apple.com/legal/privacy/). **We have no access to it**
and no ability to read, export or recover its contents.

A small number of preferences (your reminder time and reminder lead time) sync between your
devices through Apple's iCloud key-value store. These are settings, not item data.

You can disable this at any time in your device's iCloud settings, after which your data
remains on the single device.

## 3. Anonymous identifier

**When it is created.** The first time the App launches, it signs in anonymously to our
backend (Supabase) and is issued a **random identifier (a UUID)**. This happens at launch,
before and regardless of whether you use any paid or AI feature, because the same
identifier is used to check your subscription status.

**What it is.** The identifier is generated randomly. It is **not derived from and not
intentionally linked to** your name, email address, Apple Account, device identifier or any
advertising identifier. We cannot use it to work out who you are. Under UK and EU data
protection law it is nonetheless likely to count as **pseudonymous personal data**, and we
treat it as such.

**What it is used for.** Associating a request with a subscription licence, and enforcing
per-user daily limits on AI requests.

**Retention and deletion.** It persists until you delete the App and its data. You can ask
us to delete the identifier and its associated records using the contact details below.

## 4. Server-side records we hold

Our backend runs on **Supabase**. Against your anonymous identifier we store only:

| Record | Contents |
|---|---|
| Anonymous user | The random identifier and its creation timestamp |
| AI usage counter | The date, a count of requests made that day, and an estimated token total |
| Entitlement mirror | Whether Pro is active, its expiry date, and when we last checked it with RevenueCat |

Separately, and **not** linked to your identifier, we keep one app-wide tally:

| Record | Contents |
|---|---|
| Service popularity | A well-known service name (for example "Netflix") and how many devices have reported tracking it |

**We do not store the screenshots or documents you submit, the web pages you ask us to
read, the text extracted from any of them, or any of your item data.** The usage record is a
counter, not a log of content.

## 5. Information that leaves your device

### AI features (optional, Expired Pro)

Four features can send content to an AI service. Each runs only when you choose to use it:

- **Describe It and Watch quick add** — create an item from a sentence you type or speak
  (for example "Netflix, 23 dollars a month, renews on the 4th"). See "Voice input" below
  for how speech becomes text.

- **AI Screenshot Import** — creates items from a screenshot you pick or a photo you take
  with Take Photo.
- **Document Scan** — reads a document you scan, drop or open in the App (for example a
  passport, licence, insurance policy or lease) to fill in its name and dates.
- **Read Page with AI** — reads the web page at an address you enter, to fill in a
  subscription's name and price.

**With the default Analyzer setting ("Automatic"), on a device that supports Apple
Intelligence, screenshots and documents are processed on your device first**, and if that
succeeds nothing leaves it. Otherwise — if the device doesn't support it, the on-device
model can't read the content, or you have chosen a specific cloud provider under Settings →
Analyzer — the content is sent over an encrypted connection to our processing service (a
Supabase Edge Function we operate), which forwards it to **one third-party AI provider at a
time**, trying the next provider only if one is unavailable:

- For screenshots and documents, what is sent is the **image**, and/or the **text your
  device recognised in it**. A document scan can therefore include whatever the document
  shows — for example your name, date of birth and document number. **Please do not scan a
  document you would not want a third party to process.**
- For Describe It and Watch quick add, what is sent is **the sentence you typed or the
  text recognised from your speech**. Audio is never sent to our service or to an AI
  provider.
- For Read Page with AI, the App sends **the web address you entered** to our service. Our
  service then fetches that page itself, so the site sees our server's request for the page.
  Only the page's title, description and visible text are forwarded to the AI provider. Your
  device still requests the site's icon as described under "Service icons" below.

**Neither our processing service nor the App stores what you submit or the text extracted
from it.** It is held in memory only for the duration of the request and is not written to
any database or file. What our service records is a counter — see section 4.

The providers currently in use, in the order they are tried, and what each does with the
request:

**OpenAI (API)** —
[privacy policy](https://openai.com/policies/privacy-policy/) ·
[API data usage](https://openai.com/policies/api-data-usage-policies/)
OpenAI states that it does not use data sent through its API to train its models unless the
customer opts in, which we have not. API requests may be retained for a limited period (up
to 30 days under OpenAI's standard terms) for abuse and misuse monitoring, then deleted.
OpenAI is based in the United States.

**DeepSeek (Open Platform API)** —
[privacy policy](https://cdn.deepseek.com/policies/en-US/deepseek-privacy-policy.html) ·
[terms](https://cdn.deepseek.com/policies/en-US/deepseek-open-platform-terms-of-service.html)
DeepSeek's Open Platform terms are broader. DeepSeek logs API requests and associated
metadata, and its terms and privacy policy reserve rights to use inputs and outputs for
platform development, research and model improvement. **We cannot tell you that data sent
to DeepSeek is never retained or never used for model development, and we do not claim
that.** DeepSeek is based in China, so a request routed to it is processed there. DeepSeek
receives text only, never an image.

**Google (Gemini API, paid tier)** —
[privacy policy](https://policies.google.com/privacy) ·
[API terms](https://ai.google.dev/gemini-api/terms)
Google does not use prompts or generated outputs from the paid API tier to train or
fine-tune its models. Requests are retained for up to **55 days** solely for abuse and
safety monitoring, then purged.

Because a request may be processed outside the UAE, the UK and the EEA, and because the
DeepSeek terms above are broader than the others, **please do not submit screenshots,
documents or pages containing information you would not want a third party to retain.** If
you never use these features, no image, document or page content ever leaves your device.

### Voice input (microphone and speech recognition)

Describe It can listen instead of you typing, and the Apple Watch app can record a short
sentence to add an item. Both are used only when you tap the microphone or the **+** button,
and only after you grant microphone and speech-recognition permission.

- **Speech is turned into text by Apple's speech recognition, on your iPhone, iPad or Mac.**
  Where your device supports on-device recognition for your language, the App requires it
  and the audio does not leave the device. Where it does not, Apple's speech recognition
  sends the audio to Apple to be transcribed, under
  [Apple's privacy policy](https://www.apple.com/legal/privacy/). We never receive it.
- **A recording made on Apple Watch is sent only to your own paired iPhone**, which
  transcribes it and then deletes it. It is not stored and is not sent to us.
- **The resulting text** is then read on your device by Apple Intelligence where available;
  otherwise it is sent to our processing service exactly as described under "AI features"
  above.

The App does not keep recordings, and does not listen in the background.

### Widgets

If you add an Expired widget, the App shares a small list of your upcoming items (name, date,
price and icon) with the widget through storage private to the App on your device. Nothing is sent
anywhere. Lock Screen widgets never show prices, and item names are hidden while the device is
locked where the system supports it.

### Spotlight, Siri, Shortcuts and Visual Intelligence

These features work **on your device**; nothing is sent to us.

- **Spotlight.** So system search can find your items, the App adds each item that isn't
  archived to your device's on-device search index: its name, next date, price, provider,
  category or document type, website address (domain only) and icon. **Notes, document
  numbers, the holder's name, payment method and any account email, username, password or
  phone number are never indexed.** Turn this off in Settings → Privacy & Security → Show in
  Spotlight, which removes everything the App has indexed.
- **Siri and Shortcuts.** Actions such as "What's coming up" read your items on the device to
  answer. Text you give the "Add by Describing" action is handled exactly like Describe It
  (see "AI features" above).
- **Visual Intelligence (iPhone).** When you use Visual Intelligence on something and choose
  to see Expired's results, the system shares that image with the App on your device. The
  App reads its text on the device to find matching items. To offer "Add to Expired", it
  keeps a copy in its private cache for **at most 15 minutes**, and deletes it as soon as you
  open it. If you choose "Add to Expired", it goes through AI Screenshot Import as described
  above.
- **Spending recap.** The recap's summary paragraph is written on your device by Apple
  Intelligence where available. It is never sent to us or to an AI provider.

### Service icons and App Store search

To show a recognisable logo for an item, and to suggest apps as you type:

- When an item has a website address, the App requests that site's icon from public icon
  services — currently [Google's favicon service](https://policies.google.com/privacy),
  [icon.horse](https://icon.horse/) and
  [DuckDuckGo's icon service](https://duckduckgo.com/privacy) — and may also request the
  icon **directly from the website itself**. These requests contain **only the website
  domain**.
- When you search for an app while adding an item, and when the App looks up an icon by an
  item's name, **the name you typed** is sent to **Apple's App Store search service**
  (governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/)).

None of these requests contain an item's cost, dates, notes or any credentials you stored.

### Service popularity (on by default; can be turned off)

When you add an item whose name exactly matches a well-known service in the App's built-in
catalogue (for example "Netflix"), the App reports **that catalogue name** to our backend,
once per service per device, so we can see which services are most common and show them
first. **Only the catalogue name is recorded** — never a name you typed that isn't in the
catalogue, and never a cost, date, note or credential. The request travels with the
anonymous session described in section 3, but **your identifier is not stored with the
name**: the only thing kept is a per-service count (section 4).

You can turn this off at any time in **Settings → Privacy & Security → Help Improve the App**,
after which nothing more is sent.

### Exchange rates

To convert costs between currencies, the App periodically downloads current exchange rates
from our backend. The request travels with the anonymous session described in section 3,
but contains nothing about your items, and nothing about it is stored against your
identifier.

### Purchases

Expired Pro is sold through Apple's In-App Purchase. Payment is handled entirely by Apple —
**we never see or receive your payment details.** We use
[RevenueCat](https://www.revenuecat.com/privacy/) to verify subscription status; RevenueCat
receives the anonymous identifier above and the purchase receipt Apple issues, and returns
whether Pro is active. RevenueCat's SDK also collects standard device and app metadata
(such as app version, device model and operating system version) in order to validate
purchases. Subscription changes, cancellations and refunds are handled by Apple.

### Network metadata

Any internet request necessarily reveals technical information to whoever receives it. Our
backend, the icon services and websites, RevenueCat and Apple will each
receive things such as your **IP address, the time of the request, and network/user-agent
information**. We do not store, analyse or use this metadata for any purpose, and we do not
combine it with anything else; but we cannot claim the request contains nothing beyond the
content described above. Each recipient handles it under its own policy. (The AI providers
receive requests from our server, not from your device.)

## 6. What we never collect

- Your name, email address, phone number or postal address
- The account emails, usernames or passwords you store against items. **These never leave
  your device except into your own private iCloud container, and are never transmitted to
  us or to any AI provider.**
- Crash reports or performance telemetry, and any analytics beyond the anonymous
  service-popularity tally described in section 5
- Advertising or tracking identifiers
- Your location
- Your contacts, photo library, calendar or health data

## 7. How we use information

We use the limited information described above only to provide the feature you requested,
to enforce fair-use limits, to verify access to paid features, and — for the anonymous
service-popularity tally — to decide which services the App suggests first. We do not profile you,
and we do not use your information for advertising or marketing.

## 8. Retention

We do not retain your item data, because we never receive it. We do not retain the
screenshots, documents or pages you submit, or the text extracted from them. AI usage
counters are kept only as
long as needed to enforce daily limits and understand aggregate load. Entitlement records
are kept for as long as necessary to honour your purchase. The service-popularity tally holds
no identifier, so it cannot be traced back to you or deleted per person. You may request
deletion of the other records in section 4 at any time.

Retention **by the AI providers** is governed by their own terms, summarised in section 5:
up to 30 days for abuse monitoring at OpenAI, up to 55 days at Google, and per DeepSeek's
Open Platform terms for DeepSeek.

## 9. Your choices and your rights

Because your item data is held on your device and in your own iCloud container, you control
it directly:

- **Delete any item** at any time within the App.
- **Delete everything** by deleting the App and, if you used iCloud sync, removing Expired's
  data from iCloud in your device settings.
- **Keep content on your device** by not using AI Screenshot Import, Document Scan or Read
  Page with AI (in the default Automatic mode on a device with Apple Intelligence, screenshots and documents are read on
  the device first), by not entering website addresses, and by not searching the App Store
  from the add screen.
- **Turn off the service-popularity tally** in Settings → Privacy & Security → Help Improve the
  App.
- **Keep your items out of system search** with Settings → Privacy & Security → Show in
  Spotlight.
- **Withdraw consent** for the optional AI features simply by not using them; nothing is
  retained.

Some requests are part of how the App works and are not optional: the anonymous sign-in and
subscription check (sections 3 and 5, Purchases) and the exchange-rate download. None of
them carries your item data.

If you are in the United Kingdom, the European Union or another region granting
data-protection rights — access, correction, erasure, portability, restriction or objection —
you may exercise them by contacting us below, and we will respond within the period the
applicable law requires. For almost all of your data we hold no copy, so deleting it within
the App is both faster and more complete than a request to us.

## 10. Security

We use reasonable technical and organisational safeguards to protect the limited information
we hold, including encrypted transport and access controls on our backend. However, **no
method of electronic storage or transmission is completely secure**, and we cannot guarantee
absolute security.

## 11. Children

Expired is not directed to children under 13, and we do not knowingly collect personal
information from children.

## 12. Changes to this policy

If this policy changes materially, we will post the updated version at this URL with a new
effective date before the change takes effect.

## 13. Contact

Questions about this policy, or a data-protection request:
**expired.support@sixshot.app**

---
