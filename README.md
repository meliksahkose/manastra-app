# Manastra — personal affirmations with an AI coach

> A handful of affirmations written around your life each day, a 90-second evening ritual, and a coach that answers in your own words.

**iOS** · [App Store](https://apps.apple.com/us/app/manastra-daily-affirmations/id6804745346) · [manastra.melberlabs.com](https://manastra.melberlabs.com) · Designed and built end to end by [İbrahim Melikşah Köse](https://github.com/meliksahkose) at [MelberLabs](https://melberlabs.com)

<p>
  <img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource211/v4/c8/e9/18/c8e918da-1f8b-aaeb-3d2d-e9a20febc67e/01-written-for-you.png/320x480bb.jpg" width="24%" alt="Written for you" />
  <img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/19/22/29/19222906-c529-cc38-bc13-b02dec471fe3/02-evening-ritual.png/320x480bb.jpg" width="24%" alt="Evening ritual" />
  <img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/06/2e/4f/062e4fa7-f2ca-fb7c-12c0-c68b8ebe40af/03-star-map.png/320x480bb.jpg" width="24%" alt="Star map" />
  <img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/92/50/be/9250be49-3f09-7883-7e73-b8c85ae4769b/04-coach.png/320x480bb.jpg" width="24%" alt="AI coach" />
</p>

## What it does
- **LLM-generated daily affirmations** shaped by focus areas, mood and the people who matter to the user.
- **90-second evening ritual**: breathe, read, seal the intention.
- **Star map instead of a streak counter.** Every ritual adds a star, and "wish tokens" cover missed days without guilt.
- **AI coach** for everyday motivation, with clear boundaries: it is not a substitute for professional support.
- **Six languages** (EN, TR, ES, PT, DE, FR), including the voice that reads affirmations aloud.

## Engineering decisions
- **Privacy by construction.** Names, family, city and work stay on the device. Only anonymised signals (focus areas, mood, age range) reach the model. Real names are filled back in **on the phone** after generation.
- **No dark patterns.** The paywall states what you get, the price and how to cancel. The free tier stays usable.
- **Stack:** React Native (Expo) client · Node.js backend · LLM generation · auto-renewing subscriptions (weekly, monthly, yearly).

---
<sub>Source code is private. Happy to walk through the architecture and code in an interview: meliksah.kose1@hotmail.com</sub>
