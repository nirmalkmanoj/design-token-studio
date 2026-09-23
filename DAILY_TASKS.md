# Flexible daily tasks

This is the day-to-day companion to [LEARNING_PLAN.md](LEARNING_PLAN.md). Follow its guided-snippet teaching method: explain the concept and exact file location, provide a small snippet, wait while Nirmal implements and runs it, then review. Do not implement learning-project code automatically.

## How to follow this

- These are 48 numbered **learning days**, not calendar dates. A separate daily progress reminder follows the checklist; the schedule never determines which learning day is due.
- Each day has **three tasks total**: build, practice/verify, and close. Explanations and code snippets are part of the build task, not extra homework.
- Aim for about 90–150 minutes when available. A learning day can take multiple sittings. Stop sooner if attention drops or a concept needs more time.
- Missed a day? Resume the first unchecked task. No backlog, penalty, doubled workload, or need to restart.
- Have only 20–30 minutes? Complete one small snippet or investigation, record the stopping point, and leave the day in progress.
- After a longer break, use the first 10 minutes to run the app, read the last note, and explain the last feature. This replaces some build time; it is not a catch-up assignment.
- If a task is too large, split that learning day into A/B continuations, with 2–4 tasks on each continuation. Preserve the remaining plan and learning coverage.
- Do not mark a task complete until it was actually attempted and verified. A finished feature does not prove its concepts are understood.

### What “Close” means below

AI prepares the complete session document required by the master plan: explained snippets, file locations, concepts, actual result, exercise feedback, debugging, checks, and next step. AI updates the concept tracker and next-session note. Nirmal reviews the summary and diff; together we save an appropriate Git checkpoint and push when the remote is configured and available. Report exact status; never claim an unperformed push. This is **task 3**, not additional tasks.

On a partial day, document the actual stopping point. Keep unfinished work clearly identified, and use a descriptive checkpoint if committing it. If there is no new meaningful change, do not create an empty commit. Establish repository destination and visibility before the first remote publication.

## Current progress

- Next: **Day 3 — close the layout and spacing session**
- Status: Day 3's Grid/Flexbox layout, box-model inspection, temporary padding edit, and selector explanations are verified. Documentation review and the Git checkpoint remain.
- Last completed day: Day 2.
- Resume at: Review the Day 3 documentation and diff, then commit and push the layout checkpoint.
- Blockers / concepts to revisit: A local development server and starting/stopping its process remain to be practiced when needed.

Update this block at the end of each sitting. Record actual dates inside session notes; leave these day numbers unchanged.

## Progress-based reminders and completion

Schedule: **daily at 2:00 PM, Asia/Kolkata (IST)**, in the existing learning task. Automation ID: `daily-design-engineering-learning-check-in`.

- The task checkboxes are the source of truth. Select the earliest day containing an unchecked task, then resume its first unchecked task. Later checked tasks stay completed.
- During an interactive learning session, change a task to `[x]` only after the learner confirms completion or the session establishes that its actual work and checks are complete. Providing a snippet, writing a reminder, elapsed time, or a generated feature is not completion.
- Mark a learning day complete only when all three tasks are checked. Update Current progress and the next-session note at each stopping point. Record the actual activity date in the session document.
- The scheduled check reads this file, the master plan, and the latest available learning notes. It does not implement code, run a lesson without the learner, commit/push, or check off tasks on its own.
- If the previous calendar day has no recorded work, say there is no recorded progress; do not assume the learner did nothing. Keep the same unfinished task and do not add catch-up work.
- If a day is partially complete, remind only about its remaining tasks. If the learner already completed a learning day today, acknowledge the progress and offer the next day as optional, not due.
- Send one concise scheduled check-in with the current project/day, first unfinished step, and remaining checklist (at most three tasks). A partial day may have just one remaining task; do not invent more work.
- If files are unavailable or notes conflict with checkboxes, report the uncertainty and preserve checkboxes until clarified. Never infer completion just from the presence of project files.
- When all tasks are checked, announce completion once and pause the reminder using the automation tool. Do not archive this learning task.

## Project 1 — design-token studio in HTML, CSS, JavaScript

### Day 1 — first working page
- [x] **Build:** Inspect the editor/setup, create a project folder and HTML/CSS/JS starter files, and run a minimal page from explained snippets. Learn paths, tabs, terminal, localhost, and start/stop commands as needed.
- [x] **Practice:** Find and change a heading, connect one CSS rule, and inspect the browser result. Explain each file's role.
- [x] **Close:** Write day-1 notes and a README, initialize Git with a first checkpoint, and record day 2's starting point.

### Day 2 — semantic preview interface
- [x] **Build:** Add navigation, a card, buttons, a badge, and labeled form controls. Learn elements, attributes, nesting, landmarks, heading hierarchy, links/buttons, input types, and native validation.
- [x] **Practice:** Correct one inappropriate element, check keyboard order and labels, and explain image alternatives if the preview includes an image.
- [x] **Close:** Document and commit; establish the GitHub repository/visibility and push when available.

### Day 3 — layout and spacing
- [x] **Build:** Arrange the controls and preview using Grid/Flexbox. Learn normal flow, box model, dimensions, spacing, and selectors in the actual layout.
- [x] **Practice:** Inspect a box in developer tools, alter its padding, and explain the difference between padding and margin.
- [ ] **Close:** Save explained layout snippets, checks, and the Git checkpoint.

### Day 4 — responsive styling and tokens
- [ ] **Build:** Add flexible sizing, a narrow-screen layout, typography, and initial CSS custom properties. Learn units, media queries, inheritance, cascade, and specificity.
- [ ] **Practice:** Fix deliberate overflow and an overridden rule using browser Styles; predict which elements change when a spacing token changes.
- [ ] **Close:** Record the diagnosis and token explanations; commit/push.

### Day 5 — first live color control
- [ ] **Build:** Connect a labeled color input to a preview CSS variable. Learn variables, values, DOM selection, functions, parameters, and events.
- [ ] **Practice:** Trace input → handler → CSS property → screen, then wire a second color with hints rather than a complete answer.
- [ ] **Close:** Save the execution walkthrough and concept evidence; commit/push.

### Day 6 — spacing, radius, and type controls
- [ ] **Build:** Add range/number controls with a theme object, sensible defaults, and bounds. Learn types, conversion, comparisons, conditions, function returns, and scope.
- [ ] **Practice:** Diagnose a string/number mistake and add one small control variation.
- [ ] **Close:** Document control behavior, invalid-input checks, and Git status.

### Day 7 — presets and interaction states
- [ ] **Build:** Add a few presets and hover/focus/disabled styles with restrained transitions and reduced-motion behavior. Learn arrays, iteration, find/map, object copying, and primitive versus semantic tokens.
- [ ] **Practice:** Add a preset and explain which semantic roles change; verify focus and reduced-motion behavior.
- [ ] **Close:** Record state-versus-preview explanations and commit/push.

### Day 8 — save, restore, and reset
- [ ] **Build:** Save named themes locally and restore them after refresh. Learn JSON, record IDs, local storage, defaults, and error handling.
- [ ] **Practice:** Test reset and malformed saved data; explain what local storage cannot guarantee.
- [ ] **Close:** Save persistence snippets and test results; commit/push.

### Day 9 — export and organize
- [ ] **Build:** Export CSS and JSON, separating theme data from interface updates where useful. Learn serialization, downloads, modules, and imports.
- [ ] **Practice:** Inspect the exported values and safely undo a small practice change through Git.
- [ ] **Close:** Document the export path, update setup instructions, and commit/push.

### Day 10 — ship project 1
- [ ] **Build:** Fix the most important remaining issue and publish the small completed studio from a reviewed branch/PR.
- [ ] **Practice:** Check narrow screens, keyboard use, save/reset/export, and explain one entire control-to-preview flow. Practice revert in a safe branch if not yet covered.
- [ ] **Close:** Complete the project review, demo link, concept gaps, and verified Git/deployment status.

## Project 2 — travel shortlist in HTML, CSS, JavaScript

### Day 11 — Vite setup and destination cards
- [ ] **Build:** Create a vanilla Vite project with mock destination cards. Learn Node/npm/Vite, package.json, scripts, dependency types, lockfile, and .gitignore.
- [ ] **Practice:** Explain and run dev/build/preview commands; trace one module import.
- [ ] **Close:** Write the brief and README, document setup, and establish the repository checkpoint.

### Day 12 — local shortlist
- [ ] **Build:** Add/remove mock destinations and filter the list, reusing HTML/CSS/JS concepts with fewer hints.
- [ ] **Practice:** Propose the record shape, add a filter, and diagnose an incorrect record selection using stable IDs.
- [ ] **Close:** Record reinforced concepts and commit/push.

### Day 13 — first real API request
- [ ] **Build:** Choose a suitable browser-compatible API and replace mock search with fetch. Learn URLs, query parameters, HTTP, JSON, promises, and async/await.
- [ ] **Practice:** Inspect a Network request and explain its response/status and where the returned data becomes cards.
- [ ] **Close:** Document the API choice, configuration, and request path; commit/push.

### Day 14 — loading and failure states
- [ ] **Build:** Add loading, empty results, errors, and retry. Learn response.ok, try/catch, network versus HTTP failures, and basic CORS.
- [ ] **Practice:** Simulate a failure or offline response and verify recovery without losing the saved shortlist.
- [ ] **Close:** Record failure evidence and actual checks; commit/push.

### Day 15 — responsive search
- [ ] **Build:** Add debouncing and prevent outdated responses from replacing current results. Learn timers, closures, request ordering, and cancellation.
- [ ] **Practice:** Explain a stale-response scenario and verify that rapid searches show the latest result.
- [ ] **Close:** Preserve the timing explanation, debugging evidence, and Git checkpoint.

### Day 16 — destination details
- [ ] **Build:** Show one useful detail such as weather for the selected place, with accessible expand/collapse behavior and clear request states.
- [ ] **Practice:** Trace selected destination → request → detail view; test missing data and a slow response.
- [ ] **Close:** Record the second use of asynchronous concepts and commit/push.

### Day 17 — notes and persistence
- [ ] **Build:** Save notes, shortlist entries, and a display preference. Reinforce JSON/storage, event delegation, and safe rendering of entered text.
- [ ] **Practice:** Find a deliberately broken handler and verify restored data after refresh.
- [ ] **Close:** Document persistence limits and user-input handling; commit/push.

### Day 18 — budget estimate
- [ ] **Build:** Calculate an estimated trip cost from simple inputs. Learn reduce, pure functions, validation, conversion, and number formatting.
- [ ] **Practice:** Predict totals for normal/empty/invalid inputs and fix a string-concatenation bug.
- [ ] **Close:** Save calculation examples and commit/push.

### Day 19 — tests and code checks
- [ ] **Build:** Add a few meaningful Vitest calculation tests, formatting, and linting.
- [ ] **Practice:** Make a test fail for the right reason, fix it, and explain formatting versus linting and a real warning.
- [ ] **Close:** Record commands/results, dependency reasons, and commit/push.

### Day 20 — ship project 2
- [ ] **Build:** Resolve a small practice merge conflict, review the release changes, and deploy the production build.
- [ ] **Practice:** Check API failure/retry, budgets, persistence, keyboard/mobile behavior, and confirm no secrets are exposed in client configuration.
- [ ] **Close:** Finish the walkthrough, demo/README, concept gaps, and Git/deployment record.

## Project 3 — design-token studio rebuilt in React

### Day 21 — React preview skeleton
- [ ] **Build:** Start a React/Vite project and recreate the first preview using familiar CSS. Learn JSX, components, props, and composition.
- [ ] **Practice:** Draw a small component tree and map one vanilla responsibility to React.
- [ ] **Close:** Record the comparison, setup, and repository checkpoint.

### Day 22 — first stateful control
- [ ] **Build:** Make a color control update the preview through state. Learn event handlers, controlled inputs, and rendering.
- [ ] **Practice:** Trace a keystroke/change through state to the rendered result; add one control variation.
- [ ] **Close:** Save the state-flow explanation and commit/push.

### Day 23 — complete theme editing
- [ ] **Build:** Recreate radius/spacing/type controls and preset lists. Learn immutable updates, shared state, conditional rendering, and stable keys.
- [ ] **Practice:** Choose a state owner, diagnose an identity/key problem, and remove a duplicated derived value.
- [ ] **Close:** Document actual exercises and commit/push.

### Day 24 — TypeScript in the theme model
- [ ] **Build:** Add types for themes, controls, props, and callbacks. Learn inference, objects, unions, optional values, and narrowing.
- [ ] **Practice:** Fix a real type error without suppression and explain why imported JSON still needs runtime checking.
- [ ] **Close:** Save typed examples and commit/push.

### Day 25 — save, restore, and export in React
- [ ] **Build:** Recreate persistence/reset/export with a small reusable hook where justified. Learn effects, dependencies, and separation of events from synchronization.
- [ ] **Practice:** Explain why derived previews need no effect; verify saved settings after refresh and export accuracy.
- [ ] **Close:** Document effect reasoning and checks; commit/push.

### Day 26 — refs and cleanup
- [ ] **Build:** Add useful focus behavior and a timed saved-status message. Learn refs, timer cleanup, and stale closures in context.
- [ ] **Practice:** Test repeated saves and unmount/navigation behavior; explain a cleanup function.
- [ ] **Close:** Record the lifecycle trace and commit/push.

### Day 27 — Tailwind styling
- [ ] **Build:** Introduce Tailwind and restyle the app using utilities, responsive/state variants, and theme values.
- [ ] **Practice:** Translate familiar CSS rules, adjust a token, and compare the responsive result with project 1.
- [ ] **Close:** Record what Tailwind adds and the setup changes; commit/push.

### Day 28 — accessible theme dialog
- [ ] **Build:** Add a theme-editing dialog using an established component primitive.
- [ ] **Practice:** Verify labels, Tab behavior, Escape, focus restoration, and what the library does versus your code.
- [ ] **Close:** Document the component API and accessibility checks; commit/push.

### Day 29 — preview gallery and routes
- [ ] **Build:** Add a small component-preview gallery and routes with shareable selection/filter parameters.
- [ ] **Practice:** Explain URL versus local state; verify browser Back and direct-link refresh.
- [ ] **Close:** Save routing decisions and commit/push.

### Day 30 — behavior tests
- [ ] **Build:** Add selected logic/component tests and one Playwright edit/save workflow.
- [ ] **Practice:** Explain the assertions and demonstrate a meaningful regression they catch.
- [ ] **Close:** Record test commands and actual results; commit/push.

### Day 31 — automated checks and final fixes
- [ ] **Build:** Configure appropriate lint/type/build/test checks in GitHub Actions and fix one review issue.
- [ ] **Practice:** Read a failed check, find its cause, and rerun the relevant verification. Investigate performance only if there is a concrete issue.
- [ ] **Close:** Record CI evidence, unresolved limitations, and commit/push.

### Day 32 — ship and compare implementations
- [ ] **Build:** Deploy the complete React studio and finish any core feature missing from the vanilla version.
- [ ] **Practice:** Walk through both implementations; explain components/state/effects/types, and check accessibility, routing, persistence, and exports.
- [ ] **Close:** Publish the implementation comparison, final concept review, demo/README, and Git status. Storybook remains optional for a later day.

## Project 4 — personal resource library in Next.js

### Day 33 — brief, data model, and setup
- [ ] **Build:** Define resources/collections and a small scope, then scaffold Next.js with TypeScript/Tailwind and mock data.
- [ ] **Practice:** Explain the project folders, package scripts, and proposed IDs/relationships.
- [ ] **Close:** Save the brief/data model, setup notes, and repository checkpoint.

### Day 34 — pages and navigation
- [ ] **Build:** Add collection/resource pages, layouts, dynamic routes, links, and basic metadata.
- [ ] **Practice:** Trace a URL to its page and verify direct navigation and missing-record behavior.
- [ ] **Close:** Document routing conventions and commit/push.

### Day 35 — browser and server boundaries
- [ ] **Build:** Separate server-rendered content from interactive search/controls. Learn Server/Client Components, hydration, serialization, and browser-only APIs.
- [ ] **Practice:** Identify where selected code runs and what is sent to the browser; explain why Client Components are not necessarily browser-rendered only.
- [ ] **Close:** Save the execution diagram/explanation and commit/push.

### Day 36 — database connection
- [ ] **Build:** Select/configure a managed provider, create the initial schema, and read sample resources through appropriate server access.
- [ ] **Practice:** Trace one stored record to the UI and distinguish public configuration from secrets.
- [ ] **Close:** Document schema/configuration without secret values and commit/push.

### Day 37 — create resources
- [ ] **Build:** Add a server-backed create form with runtime validation and pending/error/success states.
- [ ] **Practice:** Submit invalid data and repeated clicks; verify that server validation and duplicate-submission handling work.
- [ ] **Close:** Record the mutation path and checks; commit/push.

### Day 38 — edit and delete resources
- [ ] **Build:** Add update/delete with clear user feedback and recovery from failures. Keep development data fictional while access controls are unfinished.
- [ ] **Practice:** Trace UI → mutation → database → UI and diagnose an intentionally failed update.
- [ ] **Close:** Document CRUD behavior, limitations, and commit/push.

### Day 39 — sign-in and sessions
- [ ] **Build:** Add sign-in/sign-out with the managed provider. Learn sessions, cookies, and protected navigation.
- [ ] **Practice:** Check refresh/sign-out behavior and explain authentication versus authorization.
- [ ] **Close:** Save the session explanation and configuration notes; commit/push.

### Day 40 — ownership and access rules
- [ ] **Build:** Enforce resource ownership and private access at the trusted data/server boundary.
- [ ] **Practice:** Use two test accounts and direct requests/URLs to verify that private reads and mutations are denied to the wrong user.
- [ ] **Close:** Document actual access tests and unresolved risks; commit/push. Arrange experienced review before sensitive real use.

### Day 41 — collections and filters
- [ ] **Build:** Organize resources into collections with tags/search, using the relationships defined earlier.
- [ ] **Practice:** Follow one relationship query and verify empty collections and invalid resource references.
- [ ] **Close:** Save data-model refinements and commit/push.

### Day 42 — intentional public sharing
- [ ] **Build:** Add private/public collection controls and public collection pages using fictional content.
- [ ] **Practice:** Verify what a signed-out visitor sees and that switching back to private removes access through direct URLs too.
- [ ] **Close:** Record visibility rules and checks; commit/push.

### Day 43 — caching and fresh data
- [ ] **Build:** Ensure mutations and visibility changes refresh affected views. Learn caching, staleness, and revalidation for the chosen implementation.
- [ ] **Practice:** Reproduce a stale view and explain which source of truth and cache require attention.
- [ ] **Close:** Preserve the diagnosis and verified fix; commit/push.

### Day 44 — tests and checks
- [ ] **Build:** Add a few critical workflow tests and suitable automated checks.
- [ ] **Practice:** Review assertions for add/edit and access behavior; explain what the tests do not cover.
- [ ] **Close:** Record test results, limitations, and commit/push.

### Day 45 — deploy and inspect logs
- [ ] **Build:** Configure a preview/production deployment with correct environment settings and schema requirements.
- [ ] **Practice:** Trace a controlled failure through browser, server, or build logs; verify a recovery path without damaging live data.
- [ ] **Close:** Save deployment/runbook notes, demo link, and actual Git/deployment status.

### Day 46 — accessibility and performance
- [ ] **Build:** Fix the most important keyboard/responsive issue and one observed image/font/layout-shift or loading issue.
- [ ] **Practice:** Compare before/after evidence and verify public-page metadata and the main workflow on a narrow screen.
- [ ] **Close:** Document measurements/checks and commit/push.

### Day 47 — feedback and reviewed changes
- [ ] **Build:** Address one concrete issue from user testing or engineer review; if outside feedback is unavailable, use a structured walkthrough and leave external review pending.
- [ ] **Practice:** Explain the tradeoff and verify the fix without regressing the workflow.
- [ ] **Close:** Record the source of feedback, review response, and commit/push.

### Day 48 — finish and choose the next depth area
- [ ] **Build:** Finalize the strongest demo and technical walkthrough, documenting what AI supplied and what you implemented and verified.
- [ ] **Practice:** Explain the full browser/server/database flow and review concept evidence across all four implementations; identify gaps honestly.
- [ ] **Close:** Complete final project docs and Git status, then choose one next learning target based on the gaps rather than starting another broad course.

## Starting or resuming a learning day

Say: **“Continue my learning plan from the first unfinished task. Give me today's three tasks, then explain and provide the first small snippet. Wait for me to implement it.”**

The tutor reads this progress block, the master plan, current project files, and the last session note. Do not rely on remembering which day the learner should be on. If a day is split, preserve checked tasks and carry forward only the unfinished work.
