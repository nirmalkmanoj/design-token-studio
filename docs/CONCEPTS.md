# Concept tracker

| Concept | Current evidence | Status |
| --- | --- | --- |
| HTML document structure | Created a page with a head, main region, heading, paragraph, and button; explained title versus heading | Applied |
| Doctype, character encoding, viewport | Explained standards mode, UTF-8, and the phone layout viewport; answered checks | Explained |
| CSS stylesheet link and selector | Connected `styles.css` and observed the heading change color | Applied |
| CSS custom properties and inheritance | Changed a root color token and observed heading and button update | Applied |
| Two-value padding | Predicted and observed that increasing the second value makes the button wider | Applied |
| Git repository and first commit | Used `pwd` to confirm the folder, initialized Git, inspected status, ignored `.DS_Store`, staged expected files, and created the first local commit | Applied |
| Terminal and local development server | Used the terminal for basic commands; page opened directly in a browser, so the server workflow remains | Revisit |
| Semantic landmarks and heading hierarchy | Built a header, labeled navigation, main region, two sections, an article, and ordered headings from `h1` through `h3` | Applied |
| Links and buttons | Used fragment links for page navigation, submit/reset buttons for form actions, and removed a misleading navigation action after reviewing the user flow | Applied |
| Labels and form controls | Matched each label's `for` value to an input `id`; used color, range, and constrained number inputs | Applied |
| Native validation | Verified `required` and `max` errors and restored the declared value with a reset button | Applied |
| HTML nesting | Found and corrected a form that accidentally crossed from the controls section into the preview section | Applied |
| Keyboard order and focus | Tabbed through links, inputs, and buttons in DOM order and confirmed visible focus identification | Applied |
| Image alternatives | The current preview has no image; discussed descriptive alternatives for meaningful images and empty alternatives for decorative images | Explained |
| Git remotes and first push | Configured the repository author with GitHub's no-reply address, corrected unpublished commit authors, added `origin`, and pushed `main` to the public GitHub repository | Applied |
| Normal flow and layout containers | Observed that a wrapper alone leaves sections stacked, then turned that wrapper into a layout container | Applied |
| CSS Grid | Created two equal `1fr` columns for Controls and Preview with a token-driven gap | Applied |
| Flexbox | Used a column flex container for the form and a nested row flex container for its action buttons | Applied |
| CSS selectors | Compared element selectors, reusable class selectors, unique ID selectors, and a comma-separated selector group | Applied |
| Box model | Inspected Controls in Arc DevTools, verified 32px padding and a 1px border, temporarily changed padding to 8px, and distinguished internal padding from outside margin | Applied |
| Code formatting | Used Cursor's Format Document command on CSS and HTML and verified that formatting changed source whitespace without changing browser behavior | Applied |
| Predictable element sizing | Applied universal `border-box` so declared widths include padding and borders | Applied |
| Flexible container width | Used `min()` and `calc()` to cap Header/Main at 1120px while preserving 16px viewport edges; explained automatic centering and the browser's default body margin | Applied |
| Media queries | Used a desktop-first `max-width: 700px` condition to switch the Grid from two columns to one, and verified both 800px and 600px states | Applied |
| Responsive units and fluid type | Used `rem`, `vw`, and `clamp()` to create a heading with minimum, fluid, and maximum sizes | Applied |
| Typography inheritance | Defined body typography tokens, applied them through `body`, and explicitly inherited the font into native buttons and inputs | Applied |
| Attribute selectors | Targeted only the number input with `input[type="number"]` and gave it a scalable width after its value became clipped | Applied |
| Cascade and specificity | Inspected equal-specificity Grid declarations in DevTools and saw the later active media-query rule override the earlier desktop rule; selector strength remains a concept to reinforce | Explained |
| Overflow diagnosis | Deliberately forced an 800px minimum width inside a 600px viewport, located the cause in DevTools, removed it, and verified the stacked layout | Applied |
| Token impact tracing | Predicted and observed that changing `--space-medium` affected the Grid gap, panel padding, and button horizontal padding while leaving heading size unchanged | Applied |

Statuses reflect recorded exercises, not a claim of complete mastery.
