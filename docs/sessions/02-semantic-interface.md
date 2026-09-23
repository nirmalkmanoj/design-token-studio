# Session 2 — semantic preview interface

Activity: September 23, 2026.

## Intended outcome and result

The goal was to build the meaningful HTML structure for the Design Token Studio before laying it out visually. The page now contains a header with navigation, a main heading, a controls section with a form, and a component preview represented by an article. Nirmal implemented and tested the markup from explained snippets.

## Structure and semantics

- `header`, `nav`, `main`, and `section` describe the large regions of the page.
- The navigation has `aria-label="Main navigation"` so its purpose has a meaningful accessible name.
- The page uses one `h1`, section headings use `h2`, and the preview-card heading uses `h3`.
- The component preview is an `article` because it is a self-contained example inside the preview section.
- The `New` text is a `span` because it is a small inline badge without separate structural meaning.
- Fragment links such as `href="#preview"` locate the element with the matching `id="preview"` on the same page.

## Forms, labels, and validation

The controls form contains color, range, and number inputs. Each visible label is connected to its input by matching `for` and `id` values. The number input uses `min="12"`, `max="24"`, `value="16"`, and `required`. Nirmal verified the browser's missing-value and maximum-value messages and confirmed that Reset restores the declared value of 16.

The Apply tokens button uses `type="submit"`, Reset uses `type="reset"`, and Copy styles uses `type="button"`. Copy styles is intentionally inactive until JavaScript behavior is introduced.

## Debugging and product decision

The form initially opened inside the controls section but closed inside the preview section. This also placed its buttons in the preview. The closing tags and buttons were moved so the form is fully contained by the controls section.

A proposed Get started link led from the lower preview back to controls that users had already passed. Nirmal identified that the page order made this confusing. The unnecessary link was removed and the future Copy styles action was represented as a button. This demonstrated that element semantics follow a useful product behavior; a technically valid link does not make a confusing flow useful.

## Accessibility practice

Nirmal used Tab to verify that interactive elements receive focus in the same order they appear in the HTML and used Shift+Tab to move backward. The labels and input IDs match. The current preview contains no image, so it needs no image alternative. A future meaningful image should receive concise descriptive `alt` text; a purely decorative image should use `alt=""`.

## Verification and limits

The saved HTML was inspected after each structural correction. Nirmal confirmed fragment navigation, native validation, reset behavior, and keyboard order in the browser. The controls do not update the preview yet, and Copy styles has no behavior; those JavaScript features are scheduled later. Visual layout and responsive styling begin on Day 3.

## Git checkpoint and next step

The Day 2 code and documentation checkpoint is commit `6d1144d` (“Build semantic token interface”). Git was configured to use GitHub's no-reply author address, and both unpublished commits were corrected before publication. The public repository is `https://github.com/nirmalkmanoj/design-token-studio`; `origin/main` was created and the push was verified. Next: begin Day 3 with the controls/preview layout and box model.
