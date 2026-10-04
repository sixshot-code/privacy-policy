---
layout: default
title: Privacy Policy for Voxora
---
# Privacy Policy for Voxora

**Effective date: 4 October 2026**

Voxora ("the App") records voice notes on iPhone and Apple Watch, transcribes them, and can turn them into summaries, checklists and other text.

The App is published by **Deon O'Brien, Dubai, United Arab Emirates**, referred to below as "we" or "I". For privacy purposes I am the data controller for the limited processing described here.

This policy describes exactly what the App handles, what leaves your device, and what we never collect. **Because Voxora handles your voice, please read section 3 and section 4: they explain when audio or text can leave your device.**

## Summary

- **No account is required.** There is no sign-up. We never ask for your name, email address or password.
- **We run no server for this App.** I operate no backend, database or account system for Voxora, so I do not receive your recordings, transcripts or any information about you.
- **Your recordings and transcripts stay on your device**, and, if you enable iCloud, sync privately between your own devices through your Apple Account. We cannot see them.
- **We operate no analytics, crash-reporting or advertising SDKs**, and the App shows no advertising.
- **Transcription happens on your device by default.** Audio leaves your device only if you choose an online transcription engine **with your own API key**, or if Apple's speech recognition sends it to Apple on your device and language (section 3).
- **AI actions are optional.** They run on your device with Apple Intelligence, or send the transcript text to a service you chose with your own API key (section 4).
- **We never sell, rent or trade your information.**

## 1. Information stored on your device

Everything the App creates or you enter (audio recordings, transcripts, summaries and other AI output, folders, tags, prompt templates, automation settings and preferences) is stored locally on your device in the App's private storage.

**Recording.** The App records only when you start a recording, on iPhone or on Apple Watch, after you grant microphone permission. It does not listen in the background. A recording made on Apple Watch is transferred to your own paired iPhone using Apple's connectivity between your devices. I never receive it.

## 2. iCloud sync

If iCloud is enabled on your device, the App's data (including your recordings, transcripts and AI output) also syncs through **Apple's CloudKit** into your own private iCloud container, so it appears on your other devices. That container belongs to your Apple Account and is governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/). **We have no access to it** and no ability to read, export or recover its contents.

A small number of preferences sync through Apple's iCloud key-value store. These are settings, not recordings.

You can turn this off at any time in your device's iCloud settings. The App also offers an option to delete all recordings, transcripts and AI output from the device and from iCloud (Settings).

## 3. Transcription: what happens to your audio

You choose a transcription engine. There are four:

- **Apple Speech.** Uses Apple's speech recognition. Where your device supports on-device recognition for your language, it runs on the device. **The App does not force on-device recognition, so, depending on your device and language, Apple may send the audio to its servers to transcribe it.** That processing is governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/), and I never receive the audio.
- **Whisper (on device).** Transcribes on your device with no network connection. The first time you use it, the App **downloads a speech model** that runs on your device. The model files are fetched through the WhisperKit library from its public model repository (hosted on Hugging Face). That request contains no recording or transcript, but the host sees ordinary technical information such as your IP address. See [Hugging Face's privacy policy](https://huggingface.co/privacy).
- **Gemini (online, needs your Google API key).** If you choose it, **the whole audio file is sent from your device to Google's Gemini service** to be transcribed.
- **OpenAI (online, needs your OpenAI API key).** If you choose it, **the whole audio file is sent from your device to OpenAI** to be transcribed.

The two online engines are off until you add a key and choose them. Audio goes **straight from your device to the provider**, never through me. What the provider does with it is governed by **your own agreement with them and the plan or tier your key belongs to**, not by me. See [OpenAI](https://openai.com/policies/privacy-policy/) and [Google](https://policies.google.com/privacy) ([Gemini API terms](https://ai.google.dev/gemini-api/terms)). **Providers differ in how long they keep requests and whether they use them to improve their models, the terms for free and paid tiers can differ, and I cannot tell you that a provider does not retain or reuse what you send.**

**Please do not send a recording through an online engine if you would not want a third party to process it.** Do not record other people without any consent that the law requires.

## 4. AI actions (optional)

Voxora can run AI actions on a transcript, for example to summarise it, clean it up, extract a checklist or draft an email.

- **Apple Intelligence (on device, the default).** Where supported, an action can run entirely on your device and nothing leaves it.
- **Your own API key (optional).** If you add your own key for one of the services below and choose it, **the transcript text for that action** (and the prompt you or the App built from your template) is sent **from your device straight to that provider**. I do not operate a proxy, so I never see the content, your key or the result. Your key is stored in your device's **Keychain** and is never sent to me.

| Provider | Policy |
|---|---|
| OpenAI | [Privacy policy](https://openai.com/policies/privacy-policy/) |
| Anthropic (Claude) | [Privacy policy](https://www.anthropic.com/legal/privacy) |
| Google (Gemini) | [Privacy policy](https://policies.google.com/privacy) · [Gemini API terms](https://ai.google.dev/gemini-api/terms) |
| DeepSeek | [Privacy policy](https://cdn.deepseek.com/policies/en-US/deepseek-privacy-policy.html) |

**What happens to that text is governed by your own agreement with the provider, not by me.** DeepSeek is based in China, so a request sent to it is processed there. **I cannot tell you that any provider does not retain or reuse what you send, and I do not claim that.** If you do not want a transcript to reach a third party, use Apple Intelligence, or do not run AI actions.

**Some AI steps run automatically.** After a note is transcribed, the App automatically gives it a title if it has none and, by default, writes a summary. Any automation you set up also runs on its own. Each of these uses your **default AI provider**, which is **Apple Intelligence on your device unless you change it**. If you choose an online provider as your default, those automatic steps send the transcript text to it every time a note is transcribed. You can switch the default provider, turn off automatic summaries and disable automations in Settings.

## 5. Other features

- **Reminders.** If you choose to turn the tasks in a checklist into reminders, the App asks for permission to access Reminders and, **after you confirm**, adds them to the Reminders app on your device. Reminders then syncs under Apple's own terms. The App does not read your existing reminders to send them anywhere.
- **Email and sharing.** If you draft an email or export a note, the App opens the system Mail composer or share sheet. Nothing is sent until you send or share it, and I never receive it. Anything you send or share is handled by the app or service you pick.
- **Widgets and Apple Watch.** The App shares a small amount of information (such as recent note titles) with its widgets and the Watch app through storage private to the App on your devices. Nothing is sent anywhere.
- **Purchases.** The App contains no in-app purchases and does not use RevenueCat or any other purchase service.

### Network metadata

Any internet request reveals technical information (such as your IP address, the time and the app name) to whoever receives it: a provider you chose, the model host, or Apple. I do not receive or store it. Each recipient handles it under its own policy.

## 6. What we never collect

- Your name, email address, phone number or postal address
- Your recordings, transcripts or AI output
- Crash reports, analytics or performance telemetry
- Advertising or tracking identifiers
- Your location
- Your contacts, photo library, calendar or health data

## 7. How we use information

I do not collect your information, so I do not use it. The features above use information on your device, or send it where you tell the App to.

## 8. Retention and deletion

I hold nothing about you, so I retain and can delete nothing. Your data is yours to delete:

- **Delete any note, transcript or AI output** within the App at any time.
- **Delete everything** with the App's delete-all option (this also removes it from iCloud), or by deleting the App and removing Voxora's data from iCloud in your device settings.
- **Content sent to Apple or to a provider you chose** is retained or deleted under that provider's terms. Contact them to exercise rights over it.

## 9. Your rights

Because I hold none of your data, there is nothing for me to access, correct or erase on my side. If you are in the United Kingdom, the European Union, Australia, the United Arab Emirates or another region that grants data-protection rights, you may contact me below, and I will respond within the period the applicable law requires.

## 10. Security

Your data is protected by your device's own security, and API keys are stored in the Keychain. **No method of electronic storage or transmission is completely secure**, and I cannot guarantee absolute security.

## 11. Children

Voxora is not directed to children under 13, and I do not knowingly collect personal information from children.

## 12. Changes to this policy

If this policy changes materially, I will post the updated version at this URL with a new effective date before the change takes effect.

## 13. Contact

Questions about this policy, or a data-protection request:
**support@sixshot.app**

---
