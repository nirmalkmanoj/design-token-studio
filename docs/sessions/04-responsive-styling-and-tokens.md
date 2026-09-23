# Session 4 — responsive styling and tokens

Activity: September 23, 2026.

## Intended outcome and result

The goal was to make the studio adapt to wide and narrow viewports, introduce reusable typography decisions, and diagnose responsive CSS through DevTools. The page now has a centered flexible container, a two-column desktop layout that becomes one column at 700px and below, fluid heading type, inherited body typography, and form controls that use the same font. Nirmal implemented each source change and verified the responsive states in Arc.

## Predictable and flexible sizing

The universal selector applies `box-sizing: border-box`, so declared widths include content, padding, and borders. Header and Main share a flexible container:

```css
header,
main {
  width: min(1120px, calc(100% - 32px));
  margin-inline: auto;
}
```

The browser chooses the smaller of 1120px and the viewport width minus 32px. On a 1440px viewport, resetting the browser's default body margin leaves 320px, which automatic inline margins divide into 160px per side. This also keeps roughly 16px of space at each edge on a narrow viewport.

## Responsive Grid

The desktop Grid still declares two equal columns. A later conditional rule changes only the column definition on narrow screens:

```css
@media (max-width: 700px) {
  .studio-layout {
    grid-template-columns: 1fr;
  }
}
```

Nirmal verified that the panels remain side by side at 800px and stack in document order at 600px. `max-width` is used because the stylesheet starts with the desktop layout and applies the override at 700px and below. A mobile-first version could instead make one column the default and use `min-width` to enable two columns on wider screens.

## Typography, inheritance, and units

Typography values were stored as custom properties and applied on `body`. Defining a custom property alone caused no visible change; the page changed only after another declaration consumed it. Most text inherited the body font, while native form controls initially retained their browser font. A grouped `button, input` rule with `font: inherit` made them consistent.

The number input became too narrow for its value after the typography change. An attribute selector targeted that control alone and assigned a width of `5rem`, which scales with the root text size.

The heading uses `clamp(2rem, 5vw, 3.5rem)`. The browser tries the viewport-relative middle value while enforcing a readable minimum and maximum. A unitless `line-height: 1.1` scales with the heading's computed font size.

## DevTools practice

For the overflow exercise, the Grid temporarily received `min-width: 800px` while the responsive viewport was 600px. Arc's Fit to window view made the horizontal scrollbar subtle, but DevTools showed the active 800px minimum. Removing the faulty declaration restored the responsive layout.

With `.studio-layout` selected at 600px, the Styles panel showed the desktop `grid-template-columns: 1fr 1fr` declaration crossed out and the later media-query `1fr` declaration active. The selectors had equal specificity, so the active conditional rule won through source order. Different selector strengths remain worth reinforcing in later CSS work.

For the token-impact check, `--space-medium` was temporarily changed from 32px to 16px. Nirmal predicted and observed changes to the panel padding, Grid gap, and button horizontal padding, while the heading stayed unchanged. The token was restored to 32px afterward.

## Git checkpoint and next step

The responsive source and documentation were saved in the `Build responsive token interface` commit and pushed to `origin/main`. Day 4 is complete. Begin Day 5 by connecting the primary color input to visible behavior with JavaScript.
