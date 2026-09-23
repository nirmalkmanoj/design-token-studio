# Nirmal's project-led design engineering plan

## Objective and approach

Become a product designer who can direct AI-assisted implementation, understand the code and architecture, make small changes, investigate failures, and verify shipped work. Increase engineering depth through repeated application.

AI acts as a tutor and supplies small, explained code snippets. The learner types or inserts them, runs the code, and builds the feature step by step. Do not automatically edit learning-project code or complete features on the learner's behalf. Direct implementation is available when explicitly requested for a particular task. Learning happens through contextual explanations, manual implementation, prediction, modification, debugging, and review; no standalone theory weeks.

Project choices are provisional. If an idea changes, preserve its learning outcomes and update this plan before building.

| Order | Project | Stack | Purpose |
| --- | --- | --- | --- |
| 1 | Design-token studio | HTML, CSS, JavaScript | Browser foundations, styling systems, events, local state |
| 2 | Travel shortlist | HTML, CSS, JavaScript, Vite | Reinforcement, external data, asynchronous behavior, tooling |
| 3 | Design-token studio rebuilt and extended | React, TypeScript, Tailwind, Vite | Components, typed state, reusable UI, routing and testing |
| 4 | Personal resource library | Next.js, React, TypeScript, Tailwind, managed database/auth | Browser/server boundaries, persistence, permissions, deployment |

Use sessions rather than fixed weekly deadlines. Budget roughly 100–140 focused hours for small versions, learning tasks, and documentation; this is an estimate, not a readiness guarantee. A session below is a feature milestone and may span several 60–120-minute sittings. Keep its scope small; pause at a working checkpoint if needed.

## The contract for every session

Use [DAILY_TASKS.md](DAILY_TASKS.md) for the actionable sequence: 48 flexible learning days with three tasks each. Day numbers represent progress, not calendar dates. Resume unfinished work after missed days without doubling the workload. A feature milestone below may span several learning days; the daily checklist determines today's scope. End-of-session documentation and Git work are included in the day's closing task.

### 1. Orient and agree on the outcome

Read this plan, the latest session document, project README, and current repository status. Identify uncommitted changes without overwriting them. Check the previous exercise and unresolved questions.

Present a short session brief:

- Today we are creating: one observable feature.
- By the end: a concrete behavior the user can demonstrate.
- We will learn: two or three main concepts, with incidental terms explained briefly.
- Files and tools involved: what they do and why they are involved.
- Your task: one prediction, modification, or debugging exercise.
- Done means: specific checks, documentation, and a Git checkpoint.

Do not silently build ahead into subsequent sessions. Pause when the learner must predict, attempt, or explain something.

### 2. Explain in context, provide a snippet, then let me build

Explain each important concept with: a plain-language definition, the actual mechanism, a small example, its location in this project, and a common mistake. Use analogies only alongside the actual technical explanation.

For each small implementation step:

1. Explain the concept and the intended visible result before presenting code.
2. Name the exact file and where the snippet belongs. Say whether to create a file, insert code, or replace a specific existing block; include enough surrounding context to locate it.
3. Provide a short, usable code snippet for that step rather than a full feature or large file dump. Explain unfamiliar syntax, important lines, and how the snippet connects to existing code.
4. Ask the learner to predict the result, then type or insert the snippet and run it. Supply any necessary command with an explanation of what it does.
5. Stop and wait for the learner's attempt or reported result. Do not apply the snippet, silently fix the files, or advance to the next step while waiting.
6. Review the actual result and trace one execution path together. If something fails, guide the learner through evidence and hints; provide a corrected snippet when needed for them to apply.

Prefer straightforward code, native browser features, and a small dependency set. Consult current official documentation for setup and version-sensitive APIs. Snippets are guided examples; the follow-up task should check understanding beyond copying them.

Use the same guided approach for initial setup: explain folders, commands, dependencies, and generated configuration, then let the learner perform the steps. The learner may explicitly delegate setup or repetitive implementation when desired. AI may maintain learning documentation and assist with the agreed Git workflow without taking over the coding exercise. Never treat generated output as verified merely because it looks plausible.

### 3. Give a small task and wait

Rotate tasks:

- Predict what will happen before running the code.
- Modify one behavior or styling rule.
- Find the source of a visible element or state.
- Diagnose a deliberately introduced bug in a practice change.
- Explain the data flow or compare two approaches.

Offer progressive hints rather than immediately completing the task. If the learner asks for the solution, explain it and record the concept as needing another application. Do not mark competence based on AI's work.

### 4. Verify the result

Check relevant normal, empty, invalid, error, repeated-action, keyboard, responsive, and refresh behavior. Run applicable automated checks. Record what was actually tested and any remaining limitations.

Debug using: reproduce → collect evidence → state a hypothesis → make a focused change → retest. Use Elements, Console, Network, Storage, or server logs according to the failure.

### 5. Document the session

Produce one complete Markdown session document using the template below. It should be understandable later without replaying the chat. Update the cumulative concept tracker and next-session note.

Documentation describes the actual implementation and learning, not a transcript or a list of every line of code. Preserve the important teaching snippets, their file locations, explanations, expected behavior, and the learner's actual result. Distinguish snippets provided from snippets implemented and verified. Link to relevant project files.

### 6. Save and synchronize

Inspect the diff together; identify source, generated, and unrelated files. Stage only intentional work. Commit a useful checkpoint, then push to the intended remote branch once its repository and visibility are established.

Git saves versions locally; GitHub is the remote service. Commit and push are separate actions. Use feature branches and pull requests for completed milestones as the learner becomes comfortable.

Do not publish personal records, credentials, or unrelated files. Use sample data. Never discard unrelated work, force-push, or delete branches merely to simplify the lesson. If a push is blocked by authentication or permissions, report it accurately and give the exact next step.

### 7. Close with the next step

End each session with: working result, concepts practiced, task feedback, checks, documentation link, commit/push status, open questions, and the next feature with its purpose. Do not start that next feature until the next learning session.

## Project 1 — design-token studio

### Minimum finished product

A controls panel changes a live sample interface containing buttons, a card, form fields, badges, and navigation. Users can edit a small palette, spacing, radii, and typography; reset settings; save named themes locally; and export CSS/JSON. It works on narrow screens and with a keyboard.

Begin with flat, clearly named tokens. Introduce primitive versus semantic tokens through a concrete need, such as mapping a palette value to primary actions. Do not start with a universal token architecture or Figma integration.

| Session | Build and end result | Learn and practice |
| --- | --- | --- |
| 1. Environment and first page | Create the project folder, three starter files, local preview, README, and first Git checkpoint | Editor folders/tabs/search/terminal/diagnostics/source control; paths; start/stop process; localhost; HTML/CSS/JS responsibilities. Locate and change one visible label. Establish the intended GitHub repository before the first push. |
| 2. Semantic preview interface | Build the sample interface and labeled controls | Document structure, elements, attributes, nesting, landmarks, headings, lists, links/buttons, forms, labels, images/alternatives, native validation. Correct an inappropriate element and test keyboard navigation. |
| 3. Responsive layout and initial tokens | Arrange controls beside the preview; adapt at narrow widths | Selectors, cascade, specificity, inheritance, box model, normal flow, dimensions, overflow, positioning, Flexbox/Grid, units, media queries, typography, CSS custom properties. Fix overflow and explain an overridden declaration. |
| 4. Live theme controls | Change color, radius, spacing, and font settings live | Variables, types, comparisons, objects, functions, parameters/returns, DOM selection, events, input conversion, conditions. Trace input → value → CSS variable → rendered style; add one control. |
| 5. Presets and component states | Switch presets; show hover, focus, disabled and selected styles | Arrays, iteration, map/find, object copying, state versus rendered output, semantic tokens, transitions, reduced motion. Predict which components a token change affects. |
| 6. Save, reset, and export | Save named themes, restore on refresh, export CSS/JSON | JSON, local storage, IDs, errors, defaults, downloads, scope and modules when useful. Test malformed saved data and reset behavior. Explain local storage's limits. |
| 7. Review and publish | Ship a tested first version with a short walkthrough | Diff/stage/commit/branch/push/pull/PR; safe undo and revert; static deployment; keyboard and responsive checks. Explain the whole control-to-preview path. |

Gate: locate the relevant code, explain the browser flow, change a token/control, diagnose a basic layout or event problem, and recover a working Git version.

## Project 2 — travel shortlist

### Minimum finished product

Search destinations using a suitable public API, inspect useful information such as weather, save a shortlist with notes, filter it, and calculate a simple estimated budget. Keep personal data local. No bookings, payments, maps, or accounts in the initial scope.

Choose the API at implementation time after checking browser support, keys, limits, and terms. Start with mock data so learning can continue during an API outage.

| Session | Build and end result | Learn and practice |
| --- | --- | --- |
| 1. New repository and shell | Set up a vanilla Vite app and responsive destination cards | Node/npm/Vite roles, package.json, scripts, dependencies/dev dependencies, lockfile, .gitignore, dev/build/preview, modules/imports. Explain the setup and implement a layout with fewer hints than project 1. |
| 2. API-powered search | Fetch and display destinations | HTTP, URLs, query parameters, status codes, JSON, promises, async/await, fetch, response.ok, try/catch, basic CORS. Find a request in Network and explain its response. |
| 3. Reliable request states | Loading, empty, failure, retry, and responsive search | Asynchronous ordering, debouncing, closures, timers, stale responses, cancellation. Reproduce a race or failure and verify its resolution. |
| 4. Shortlist and preferences | Save destinations, notes, filters, and display preferences | Arrays/objects, filter/find/map, IDs, event delegation, persistence, data/render separation, safe text rendering. Add a filter and fix a broken handler. |
| 5. Budget calculator | Compute an estimated total with validated inputs | Conversion, pure functions, reduce, edge cases, number/currency formatting. Find a string-concatenation bug; use Vitest to check meaningful calculation examples. |
| 6. Quality and deployment | Format/lint, build, test and publish | Formatting versus linting, error stacks, API failures, secrets versus client configuration, dependency judgment, Git conflict practice. Review a PR and verify the deployed build. |

Gate: understand a new data model, trace a request, investigate failures, explain asynchronous behavior, and apply HTML/CSS/JS foundations in a second project.

## Project 3 — rebuild and extend the design-token studio

### Minimum finished product

Rebuild all core project-1 features in React. Preserve the original for comparison. Then add a component-preview gallery, richer theme editing, and shareable preview routes. Do not add every potential feature.

Introduce React with familiar CSS first, TypeScript after the initial working interaction, then Tailwind. This progression happens inside the project, not in standalone study phases.

| Session | Build and end result | Learn and practice |
| --- | --- | --- |
| 1. React skeleton and first preview | Set up Vite/React and recreate the initial layout | JSX, components, props, composition, imports, component tree. Map vanilla code to React responsibilities. |
| 2. Interactive theme editing | Recreate controls and preset switching | State, handlers, rendering, controlled inputs, conditional rendering, stable keys/identity, immutable updates, lifting state, derived values. Choose the state owner and remove a duplicated value. |
| 3. Type the theme model | Add types to records, controls, and callbacks | Inference, object/prop/function types, unions, optional values, narrowing; compile-time types versus runtime validation. Resolve a real type error without suppression. |
| 4. Persistence and reusable logic | Restore themes, focus controls, share persistence behavior | Effects for external synchronization, dependencies, cleanup, refs, custom hooks; stale closures when encountered. Explain why filtering needs no effect but storage synchronization may. |
| 5. Tailwind and reusable UI | Restyle the app and add an accessible edit dialog | Utilities, variants, theme values, CSS relationships, component primitives, focus management. Check Escape, focus restoration, labels, and keyboard navigation. |
| 6. Preview gallery and routes | Add preview pages and shareable selection/filter URLs | Router, paths/parameters, history, URL versus component state, composition, context only if shared state warrants it. Verify refresh and Back. |
| 7. Tests and automated checks | Protect a core edit/save/export workflow | Vitest for logic, React Testing Library for selected behavior, Playwright for a critical browser flow; lint/type/build/test checks in CI. Explain what a test would catch. |
| 8. Polish and comparison | Publish the rebuild and explain differences from vanilla | Accessibility review, performance investigation when evidence warrants it, reusable component documentation, reviewed PR. Optional Storybook example, not a release requirement. |

Gate: explain component boundaries and state ownership, diagnose rendering/key/effect issues, read types, and compare both implementations concretely.

## Project 4 — personal resource library

### Minimum finished product

Save links with titles, notes, tags, and collections. Sign in to manage your library. Keep collections private or deliberately publish selected collections. Include search/filtering and public collection pages. Defer uploads, team collaboration, payments, automatic URL scraping, and AI features.

Use Next.js App Router with TypeScript/Tailwind and one managed database/authentication provider selected during setup. Next.js supplies its application tooling; this project does not use Vite.

| Session | Build and end result | Learn and practice |
| --- | --- | --- |
| 1. Plan and scaffold | Define records/relationships and build mock-data collection pages | Next.js project structure, app routes, layouts, dynamic segments, navigation, metadata, package scripts. Propose the data model before working through the implementation snippets. |
| 2. Rendering boundaries | Display collection data with interactive search/controls | Server/Client Components, prerendering/request rendering at an introductory level, hydration, serialization, browser-only APIs. Trace where code executes; distinguish Client Components from exclusively browser-rendered content. |
| 3. Database persistence | Read/create/update/delete resources | Tables/records/IDs/relationships, schema changes, server data access, environment variables, secrets. Trace a record from storage to UI. |
| 4. Reliable mutations | Validate forms and handle pending/error/success states | Runtime validation, server mutations, HTTP/API boundaries, duplicate submissions, source of truth. Invalid inputs must fail at the trusted server boundary too. |
| 5. Accounts and access | Sign in and restrict private resources to their owners | Sessions, cookies at a basic level, authentication versus authorization, ownership/access rules. Test two separate accounts and direct access to private records. Use an established auth provider; obtain experienced review before sensitive real use. |
| 6. Public collections and updates | Publish selected collections and keep views current | Explicit visibility, dynamic routes, caching/staleness/revalidation. Explain why a successful save might not immediately change another view. |
| 7. Ship and investigate | Deploy with correct environment configuration | Preview/production, browser/server/build logs, migrations/configuration, recovery/rollback, public metadata, images/fonts/layout shift, basic performance measurement. Diagnose a controlled failure. |
| 8. User feedback and final review | Improve one real workflow and document the project | Critical browser tests, accessibility checks, authorization verification, external code review, technical walkthrough and honest limitations. |

Gate: explain interaction → request/mutation → validation/authorization → database → updated UI, and investigate failures across those boundaries.

## Documentation structure inside each project

```text
README.md
docs/
  PROJECT_BRIEF.md
  CONCEPTS.md
  NEXT_SESSION.md
  FINAL_REVIEW.md
  sessions/
    01-setup-and-first-page.md
    02-....md
```

- README: purpose, prerequisites, install/run/check/build commands, demo link, limitations.
- PROJECT_BRIEF: user, workflow, scope, data model, stack and reasons, completion criteria.
- CONCEPTS: cumulative index with concept, plain-language summary, file/example, status, and evidence.
- NEXT_SESSION: next outcome, starting state, prerequisites, unresolved questions.
- FINAL_REVIEW: architecture/data flow, design and implementation choices, verification, feedback, AI contribution, current limits, and next improvements.

### Complete session-document template

```markdown
# Session NN — title
Date:
Project / branch:

## Intended outcome
What we planned to create and learn.

## Working result
What actually works, how to run/open it, and what remains unfinished.

## Concepts explained
For each important concept:
- Definition in plain language.
- How it works under the hood.
- Why it is used here.
- Relevant file/function and a short explained snippet if useful.
- Common mistake or limitation.

## Execution/data-flow walkthrough
Trace one actual interaction from input to visible result and persistence.

## Guided implementation
Important snippets, exact file/insertion locations, explanations, and expected results.
Record what the learner implemented and ran, what was verified, and any steps still pending.

## Files, commands, and dependencies
What changed, what each relevant file does, commands used and their purpose,
and why any dependency was added.

## Your task and feedback
Task, prediction/attempt, hints given, result, correction, and transfer question.
Distinguish completed work from exercises still pending.

## Debugging and decisions
Symptom → evidence → hypothesis → fix → verification.
Explain important implementation choices and alternatives briefly.

## Verification
Actual manual checks and automated results; failures and limitations.

## Git checkpoint
Branch, commit reference/message, push status, and PR link where applicable.
Never claim a push or check succeeded without verification.

## Learning status
Seen / Explained / Applied / Revisit, with evidence rather than confidence alone.

## Next session
Next feature, why it comes next, relevant concepts, and the first action.
```

The session document can identify the implementation commit while being finalized in a subsequent documentation commit. Avoid trying to embed a commit's own hash inside that same commit.

## Completion and boundaries

Every project ends with a working demo, readable repository, complete session notes and concept index, one documented bug investigation, relevant tests, accessibility/responsive checks, and a final implementation walkthrough. Project 3's comparison with project 1 is part of the portfolio evidence.

This covers practical frontend foundations, not all software engineering. Defer advanced algorithms, distributed systems, custom auth, Docker, complex state libraries, and advanced TypeScript until needed. Tools are selected for this path, not presented as a universal industry stack.

Keep applying for product design roles. Use the finished work to demonstrate growing implementation ownership, and evaluate design engineering roles against the code you can explain, modify, and verify.

## Current next step

Project 1, session 1: confirm the small design-token studio brief, inspect the available editor/runtime/Git setup, create the initial HTML/CSS/JS page and local preview, explain the files, give the first modification task, then document and commit the result. Establish the intended repository and visibility before publishing it to GitHub. This plan does not itself create an app or remote repository.

## Reference shelf — use when a feature requires it

- MDN foundations: https://developer.mozilla.org/en-US/curriculum/core/
- GitHub flow: https://docs.github.com/en/get-started/using-github/github-flow
- Vite: https://vite.dev/guide/
- React: https://react.dev/learn
- React effects: https://react.dev/learn/you-might-not-need-an-effect
- TypeScript: https://www.typescriptlang.org/docs/handbook/intro
- Tailwind with Vite: https://tailwindcss.com/docs/installation/using-vite
- Next.js: https://nextjs.org/docs/app

Check current official documentation during implementation rather than copying version-sensitive setup instructions from old lessons.
