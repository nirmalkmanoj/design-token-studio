# Session 3 — layout and spacing

Activity: September 23, 2026.

## Intended outcome and result

The goal was to arrange the Controls and Preview areas into a readable two-column interface and make spacing visible enough to inspect. The page now uses Grid for its two major panels, Flexbox for the form and its action row, and token-driven padding and gaps. Nirmal implemented each change, predicted the layout behavior, and verified the result in the browser.

## Layout structure

In `index.html`, the Controls and Preview sections were placed inside a shared wrapper:

```html
<div class="studio-layout">
  <section id="controls">...</section>
  <section id="preview">...</section>
</div>
```

The wrapper initially made no visual difference because a `div` participates in normal document flow and its block children remained stacked. This separated the HTML relationship from the later CSS layout behavior.

In `styles.css`, Grid created two explicit equal columns:

```css
.studio-layout {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--space-medium);
}
```

The first section occupies the left column and the second occupies the right because Grid follows their document order. Each `1fr` receives an equal fraction of the available width. Nirmal also compared this with a valid Flexbox-row alternative and understood that Grid states the equal-column intention directly.

## Flexbox and nested layout

The form uses a one-dimensional vertical Flexbox layout:

```css
form {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: var(--space-small);
}
```

The form fields remain stacked. The two actions were wrapped in `.form-actions`, which uses Flexbox's default row direction so only those buttons sit beside each other. This demonstrated that layout containers can be nested and independently control their direct children.

## Selectors and box model

Nirmal identified three selector forms in the project: `form` selects all form elements, `.form-actions` selects reusable class labels, and `#controls` selects a specific ID. Controls and Preview share a comma-separated rule:

```css
#controls,
#preview {
  padding: var(--space-medium);
  border: 1px solid #d9d9e3;
  border-radius: 12px;
}
```

Padding creates space inside the border. Margin creates space outside the border between an element and surrounding content. Grid `gap` provides spacing between grid items without adding margins to either panel.

## DevTools practice and verification

In Arc's Chromium DevTools, Nirmal selected the Controls section and inspected its computed box model. The panel showed a one-pixel border and 32px padding resolved from `--space-medium`. In the Styles panel, the padding declaration was temporarily changed to 8px. The content moved closer to the section border while the 32px Grid gap remained unchanged. Refreshing discarded the temporary DevTools edit and restored the source-defined token value.

The saved HTML and CSS were formatted with Cursor's Format Document command. The final whitespace check passed. The layout is still intentionally desktop-first; narrow-screen adaptation belongs to Day 4.

## Git checkpoint and next step

The Day 3 commit and push are pending at the time of this note. Review the source and documentation diff, save the layout checkpoint, and push it to `origin/main`. Then begin Day 4 with responsive sizing and typography.
