---
layout: default
title: Privacy Policy for SteadyState
---
# Privacy Policy for SteadyState

**Effective date: 4 October 2026**

SteadyState ("the App") is a task and to-do manager for iPhone, iPad, Apple Watch and Mac.

The App is published by **Deon O'Brien, Dubai, United Arab Emirates**, referred to below as "we" or "I". For privacy purposes I am the data controller for the limited processing described here.

This policy describes exactly what the App handles, what leaves your device, and what we never collect.

## Summary

- **No account is required.** There is no sign-up. We never ask for your name, email address or password.
- **We run no server for this App.** I operate no backend, database or account system for SteadyState, so I do not receive your tasks, notes, lists or any information about you.
- **Your tasks stay on your device**, and, if you enable iCloud, sync privately between your own devices through your Apple Account. We cannot see them.
- **We operate no analytics, crash-reporting or advertising SDKs**, and the App shows no advertising.
- **AI features are optional.** They use Apple Intelligence on your device, or, only if you add **your own** API key, a third-party AI service of your choosing. Content goes from your device **directly to that service**, never through me. See section 4.
- **We never sell, rent or trade your information.**

## 1. Information stored on your device

Everything you enter (task titles, notes, lists, tags, dates, reminders, priorities, links and settings) is stored locally on your device in the App's private database. **Reminders and notifications are scheduled and delivered locally by your device.** I operate no push-notification server, and no reminder passes through me.

If you add a SteadyState widget, Live Activity or Apple Watch app, the App shares a small amount of task information (such as task titles and dates) with them through storage private to the App on your devices. Nothing is sent anywhere.

## 2. iCloud sync

If iCloud is enabled on your device, the App's database also syncs through **Apple's CloudKit** into your own private iCloud container, so your tasks appear on your other devices. That container belongs to your Apple Account and is governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/). **We have no access to it** and no ability to read, export or recover its contents.

A small number of preferences sync between your devices through Apple's iCloud key-value store. These are settings, not task content.

You can turn this off at any time in your device's iCloud settings, after which your data remains on the single device.

## 3. Voice input

If you use voice input, the App uses **Apple's speech recognition** to turn what you say into text. You are asked for microphone and speech-recognition permission first, and the microphone is used only while you are dictating.

- On Apple Watch, recording is transcribed with on-device recognition where your device supports it for your language.
- On iPhone, iPad and Mac, **the App does not force on-device recognition**. Depending on your device and language, Apple may process the audio on its servers to transcribe it. That processing is governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/), and **I never receive the audio**.

The App does not keep recordings and does not listen in the background.

## 4. AI features (optional)

SteadyState can help you break a task into steps, suggest reminder times, build a smart list from a sentence you type, and design a colour theme from a description. Each runs **only when you choose to use it**.

**Apple Intelligence (on device).** Where your device supports it, these features can run entirely on your device, and nothing leaves it.

**Your own API key (optional).** If you enter your own key for one of the services below and choose it in Settings, the content for that request is sent **from your device straight to that provider**. I do not operate a proxy, so I never see the content, the key or the response. Your key is stored in your device's **Keychain**, on that device only, and is never synced or sent to me.

| Provider | Policy |
|---|---|
| OpenAI | [Privacy policy](https://openai.com/policies/privacy-policy/) |
| Anthropic (Claude) | [Privacy policy](https://www.anthropic.com/legal/privacy) |
| Google (Gemini) | [Privacy policy](https://policies.google.com/privacy) · [Gemini API terms](https://ai.google.dev/gemini-api/terms) |
| DeepSeek | [Privacy policy](https://cdn.deepseek.com/policies/en-US/deepseek-privacy-policy.html) |

What is sent depends on the feature:

- **Task breakdown:** the task's title and, if it has one, its notes.
- **Reminder suggestions:** the task's title, notes, due date and time, and priority.
- **Smart list from a sentence:** the sentence you typed and the names of your tags.
- **Theme from a description:** the description you typed.

When you load the list of available models, the App also contacts the provider to fetch it, using your key.

**What happens to that content is governed by your own agreement with the provider, and by the plan or tier your key belongs to, not by me.** Providers differ in how long they keep requests and whether they use them to improve their models, and the terms for free and paid tiers can differ. **I cannot tell you that a provider does not retain or reuse what you send, and I do not claim that.** In particular, DeepSeek is based in China, so a request sent to it is processed there. If you do not want a task's text to reach a third party, use Apple Intelligence or do not use the AI features.

## 5. Other requests the App makes

- **Link titles.** When you add a web link to a task, the App fetches that page **from your device** to read its title. The website therefore sees a normal request from your IP address. For YouTube links it asks YouTube's public oEmbed service for the title, and sends YouTube the link.
- **Apple services.** Notifications, iCloud and speech recognition are provided by Apple under its own policies.

I operate none of these services and receive none of these requests.

### Mac: optional local integration

The Mac app includes optional integration features that let other tools talk to the App, through a local connection and a file drop folder. **They are off until you turn them on.** By default the connection accepts requests only from your own Mac. There is an additional option to allow other devices on your local network to connect: if you turn it on, those devices can reach the App, protected by a secret token that is stored in your Mac's Keychain. I never receive anything through these features.

### Network metadata

Any internet request reveals technical information (such as your IP address, the time and the app or browser name) to whoever receives it: a website you link to, an AI provider you chose, or Apple. I do not receive or store it. Each recipient handles it under its own policy.

## 6. What we never collect

- Your name, email address, phone number or postal address
- Your tasks, notes, lists, tags or any other content you create
- Crash reports, analytics or performance telemetry
- Advertising or tracking identifiers
- Your location
- Your contacts, photo library, calendar or health data

## 7. How we use information

I do not collect your information, so I do not use it. The features above use information on your device, or send it where you tell the App to.

## 8. Retention and deletion

I hold nothing about you, so I retain and can delete nothing. Your data is yours to delete:

- **Delete any task, list or tag** within the App at any time.
- **Delete everything** by deleting the App and, if you used iCloud sync, removing SteadyState's data from iCloud in your device settings.
- **Content sent to an AI provider you chose** is retained or deleted under that provider's terms. Contact them to exercise rights over it.

## 9. Your rights

Because I hold none of your data, there is nothing for me to access, correct or erase on my side. If you are in the United Kingdom, the European Union, Australia, the United Arab Emirates or another region that grants data-protection rights, you may contact me below, and I will respond within the period the applicable law requires.

## 10. Security

Your data is protected by your device's own security, and API keys are stored in the Keychain. **No method of electronic storage or transmission is completely secure**, and I cannot guarantee absolute security.

## 11. Children

SteadyState is not directed to children under 13, and I do not knowingly collect personal information from children.

## 12. Changes to this policy

If this policy changes materially, I will post the updated version at this URL with a new effective date before the change takes effect.

## 13. Contact

Questions about this policy, or a data-protection request:
**support@sixshot.app**

---
