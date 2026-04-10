# AI FAQ Generator — WordPress Plugin

> A free AI-powered tool that generates SEO-optimized FAQ sections in seconds — no account required for end users.

🔗 **Live demo:** [mygrowthbox.com]((https://mygrowthbox.com/generateur-de-faq-optimisee/)) *(insert your page URL)*

---

## What it does

AI FAQ Generator is a online tool I built. Visitors enter a topic, a URL, or a block of text — the AI returns a fully structured FAQ they can customize and paste into any website.

No sign-up. No paid subscription. Just paste and publish.

---

## Key features

- **AI generation** via Groq, Google Gemini, Mistral or DeepSeek (free tiers)
- **URL support** — paste a domain and the plugin fetches and extracts page content automatically
- **Inline editor** — modify every question and answer before exporting
- **Visual style editor** — colors, fonts, backgrounds, all customizable
- **One-click HTML export** with:
  - `schema.org/FAQPage` JSON-LD → Google rich snippets + LLM-readable
  - WCAG 2.1 AA accordion (keyboard nav, aria attributes, focus management)
  - Zero JS dependencies — ~3 KB output
- **Options**: bold keywords in answers, inline emoji, question mark enforcement
- **Bilingual** — French and English interfaces via separate shortcodes
- **Lead capture** — logs visitor inputs to a custom DB table, exportable as CSV

---

## Tech stack

| Layer | Details |
|---|---|
| Backend | PHP 7.4+, WordPress Plugin API |
| Frontend | Vanilla JavaScript (ES5), CSS3 |
| AI APIs | Groq · Google Gemini · Mistral AI · DeepSeek |
| SEO | schema.org FAQPage JSON-LD |
| Accessibility | WCAG 2.1 AA |
| Data | Custom MySQL table, CSV export |

---

## How it works

```
User input (text or URL)
        │
        ├── URL detected → fetch page → strip HTML → extract text
        │
        ▼
Prompt builder → AI API call
        │
        ▼
JSON parser + sanitizer
  (enforce "?", strip bold from questions, limit to 1 bold group per answer)
        │
        ▼
Frontend JS
  → Editable FAQ list
  → Live style preview
  → Full HTML + JSON-LD export
  → Copy via Clipboard API
```

---

## Screenshots

*Coming soon — live demo available at the link above.*

---


> This is a proprietary project. The source code is not publicly available.

---

## Author

Built by MGB
