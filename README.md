# Zoonix

Zoonix is a local-first campaign workspace for small businesses. It includes campaign management, an editable campaign-copy generator, banner design, demo analytics, coupon management, brand settings, and light/dark/system themes.

## Run locally

```bash
npm install
npm run dev
```

Build the production bundle with `npm run build`; check lint with `npm run lint`.

## Campaign generator prototype

Open **AI Campaign Generator** from the sidebar or Overview quick actions. Enter the business and offer details, choose a goal, platform, language, and tone, then generate editable headlines, captions, a call-to-action, hashtags, and a banner preview. Copy captions, regenerate the suggestions, open the preview in Banner Studio, or save the result to Campaigns as a draft.

Content generation uses local templates in `src/campaignGenerator.ts`. It does not call an AI model, external API, or paid service. English, Hindi, and Kannada templates are included. Choosing another language displays an explicit note that the prototype falls back to English. Generated drafts and other workspace data are stored in the browser's local storage. Campaigns are not published to external platforms.
