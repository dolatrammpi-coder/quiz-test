# My Study Portal — Maintenance Guide

## Central files

- `config.js` — site name, tagline, common URLs and AdSense configuration.
- `common.js` — shared header, navigation, footer, breadcrumb and ad placeholders.
- `style.css` — site-wide visual design.

## New quiz pages

Use `quiz-template.html` as the starting point.

Keep only page-specific content in the quiz page. Add:

```html
<div data-site-header></div>
```

before the main content and:

```html
<div data-site-footer></div>
```

after it.

Also load:

```html
<script src="config.js" defer></script>
<script src="common.js" defer></script>
```

## Important

Do not add a fake AdSense publisher ID.

When the real AdSense publisher ID and ad slot IDs are available, they can be entered once in `config.js`.

Existing quiz questions and answers should remain page-specific; common site elements should stay centralized.
