# Changelog

## [5.1.0] — April 2026
- Questions now always end with `?` (prompt + server-side enforcement)
- Emoji placed inline after the relevant word, not at the start of the sentence

## [5.0.0] — April 2026
- Added item background color picker in the Style tab
- Added tooltip explaining the Accent color field
- Added "Delete all leads" button in the admin panel
- Fixed: copy-to-clipboard now works reliably across all browsers and WordPress themes
- Fixed: bold formatting can no longer appear in questions — answers only

## [4.0.0] — April 2026
- URL input support (auto-fetch and extract page content)
- Lead capture with admin view, CSV export and data deletion
- English interface via `[mgb_faq_generator_en]` shortcode
- Bold keywords option (1 group per answer)
- Inline emoji option
- 1,500 character limit with live counter
- Brand color `#9E8612` applied throughout

## [3.1.0] — April 2026
- Multi-API admin panel: switch between Groq, Gemini, Mistral, DeepSeek from WordPress Settings
- Plugin fully encapsulated in a PHP singleton class (no conflicts)
- PHP fatal errors during AJAX returned as readable JSON

## [2.0.0] — April 2026
- Style editor: colors, fonts, live preview
- HTML + JSON-LD export tab

## [1.0.0] — April 2026
- Initial release: FAQ generation via Groq API
- Editable Q&A list
- schema.org FAQPage output
- WCAG 2.1 AA accordion
