# Session 1 — first page and reusable CSS tokens

Activity: September 20–22, 2026. The page was built across several sittings.

## Intended outcome and result

The goal was to create the first page, understand its structure, connect CSS, and practice a reusable design token. `index.html` now displays a heading, paragraph, and sample button. The heading and button background use the same color token. Button padding uses two spacing tokens. Nirmal confirmed the page displays, that changing the color token updates both elements, and that increasing horizontal padding makes the button wider.

The page is opened directly from the filesystem in a browser. No local server, JavaScript behavior, Git repository, commit, or remote push has been verified yet.

## Concepts learned in the project

- `<!DOCTYPE html>` requests standards rendering. It is a declaration, not visible content.
- `<meta charset="UTF-8">` tells the browser how to decode the file's text. It supports the characters discussed, including Malayalam and emoji, when the file is saved in UTF-8.
- The viewport setting uses the device width as the mobile layout viewport and starts at a scale of one. It does not create a responsive layout by itself.
- The HTML `<title>` sets browser-tab text; `<h1>` displays the main heading in the page.
- The stylesheet link in `<head>` loads `styles.css` from beside the HTML file.
- `:root` matches the document root, which is `<html>` for this page. CSS custom properties declared there are available to descendants through inheritance.
- A CSS variable takes effect only where a property uses `var(...)`. The paragraph remained unaffected by the color token.
- In two-value padding, the first controls top/bottom and the second controls left/right.

## Guided implementation and observed behavior

In `index.html`, the initial structure included the document declaration, head metadata, title, main heading, and paragraph. The learner then added a stylesheet link in the head and a sample button in main.

In `styles.css`, a direct heading color was replaced with a shared token:

```css
:root {
  --color-primary: rebeccapurple;
}

h1 {
  color: var(--color-primary);
}
```

Changing the token to teal and then back to purple changed the heading. The sample button was styled to use the same color for its background. Nirmal confirmed both updated together while the button's white text stayed white.

Spacing was then named and applied to the button:

```css
:root {
  --space-small: 12px;
  --space-medium: 32px;
}

button {
  padding: var(--space-small) var(--space-medium);
}
```

The original medium value was 20px. Nirmal predicted that increasing it to 32px would widen the button and confirmed the result in the browser.

## Files and tools

`index.html` holds structure; `styles.css` holds presentation. `app.js` was renamed to its correct extension but remains empty. Cursor was used to edit files. The browser loaded the HTML file directly and required a refresh to show saved changes.

## Debugging and decisions

The three initial code filenames had underscores instead of extensions, and the JavaScript file later had an extra `s`. Nirmal corrected the names. Direct browser preview was used for this simple page; a local development server remains to be learned. Root-level tokens were introduced through a visible change rather than as a standalone theory exercise.

## Verification and limits

Verified by Nirmal's reported browser checks: the heading appeared, the stylesheet affected it, color-token changes updated both heading and button, and changing the second padding value widened the button. The assistant inspected the saved HTML and CSS. No automated tests, local server, or Git checkpoint have been performed.

## Git checkpoint and next step

Git checkpoint: **pending**. No repository or commit exists yet. Next, guide Nirmal through the first Git command, inspect the result, and save the initial checkpoint. Then update the Day 1 checklist and start Day 2.
