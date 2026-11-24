# Frontend Roadmap 2026-2027

From zero to solid React. Modern CSS → Tailwind → React → Router → final project.

**Started:** September 9, 2026
**Target:** January 29, 2027
**Pace:** 2 h/day, 5 days a week

---

## How to read this roadmap

Every block has three parts:

- **What I learn:** the concepts, not the tools.
- **What I build:** the project that proves it.
- **Done when:** checkable criteria. If they aren't met, it isn't done.

A project only counts as done when it is **deployed** and its README explains what it does and what I learned.

---

## Block 1 — CSS you actually use ✅

*Sep 7 – 27 · Completed*

- [x] Navbar + card + footer with Flexbox
- [x] Dashboard with Grid
- [x] **Milestone 1:** Responsive landing page + dark mode with CSS variables

---

## Block 2 — Tooling + Tailwind ✅

*Sep 28 – Oct 11 · Completed*

- [x] Base repo with Vite + ESLint + Prettier
- [x] **Milestone 2:** Milestone 1 landing page rewritten in Tailwind

---

## Block 3 — React core

*Oct 12 – Dec 20*

### 3.1 Product catalog ✅

Components, props, lists and keys.

- [x] Deployed · index-as-key bug documented in its README

### 3.2 Shopping cart (in progress)

**What I learn:** `useState`, state shared between components, immutability, passing functions through props.

**Done when:**
- [ ] Adding a product puts it in the cart with quantity 1
- [ ] Adding the same product again increases its quantity instead of duplicating it
- [ ] I can remove a product
- [ ] I can change the quantity by hand, and reaching 0 removes the product
- [ ] The total is computed automatically and shown with 2 decimals
- [ ] State lives in `App` and is never mutated (no `push`, no editing existing objects)
- [ ] An empty cart shows a message, not a blank list
- [ ] Deployed to Netlify

### 3.3 Sign-up form with validation

**What I learn:** controlled components, `onChange`, `onSubmit`, validation, showing errors.

**Done when:**
- [ ] Every field is controlled by state
- [ ] Validates: email format, password of 8+ characters, confirmation that matches
- [ ] Errors appear under their own field, not in an `alert`
- [ ] The submit button is disabled while the form is invalid
- [ ] `preventDefault()` on submit
- [ ] Every `input` has a `label` tied to it with `htmlFor`
- [ ] Deployed

### 3.4 Search with a public API — Milestone 3

**What I learn:** `useEffect`, `fetch`, async/await, loading and error states, cleanup, debounce.

**Done when:**
- [ ] Searches against a real API (PokéAPI, OMDb, whichever I pick)
- [ ] Shows a loading state while waiting
- [ ] Shows a clear message if the API fails
- [ ] Shows "no results" when nothing matches
- [ ] Does not fire a request on every keystroke (debounce around 400 ms)
- [ ] Cancels the previous request if the user keeps typing
- [ ] Deployed

---

## Block 4 — Router, persistence and quality

*Dec 21 – Jan 10*

### 4.1 Routes and navigation

**What I learn:** React Router, dynamic routes, `useParams`, `useNavigate`, 404 page.

**Done when:**
- [ ] `/` lists products, `/product/:id` shows the detail view
- [ ] Any unknown route lands on my own 404 page
- [ ] Reloading the page on `/product/3` works (configured on Netlify)
- [ ] The cart survives navigation between routes

### 4.2 Persistence

**What I learn:** `localStorage`, `useEffect` for syncing, lazy initial state.

**Done when:**
- [ ] The cart survives a page reload
- [ ] It doesn't crash if `localStorage` holds corrupted data

### 4.3 Custom hooks and cleanup

**What I learn:** extracting logic into custom hooks, recognizing when a component does too much.

**Done when:**
- [ ] Cart logic lives in `useCart()`
- [ ] Fetch logic lives in `useFetch()`
- [ ] No component is longer than ~100 lines

### 4.4 Accessibility and responsive

**Done when:**
- [ ] Everything is usable with the keyboard alone
- [ ] Images have `alt` text
- [ ] Enough contrast in both light and dark mode
- [ ] Works well at 375 px wide
- [ ] Lighthouse: 90+ on accessibility

---

## Block 5 — Final project

*Jan 11 – 29*

The one that goes at the top of the portfolio. Three rules:

1. **It solves a real problem**, ideally one from the conversations I already had.
2. **Someone else uses it**, even if it's one person.
3. **It explains itself**: a README with the problem, the decisions and screenshots.

### Week 1 (Jan 11–17): define and build the core
- [ ] Problem and user written in one sentence
- [ ] Screens sketched on paper before writing code
- [ ] Core feature working, no styling yet

### Week 2 (Jan 18–24): complete it
- [ ] Routes, forms and persistence
- [ ] Loading, error and empty states on every view
- [ ] Responsive and accessible

### Week 3 (Jan 25–29): polish and present
- [ ] Deployed with a clean URL
- [ ] README with the problem, screenshots and technical decisions
- [ ] 2-minute video in English explaining it
- [ ] At least one person used it and gave feedback

---

## Stack

| Area | Tool |
| --- | --- |
| Language | JavaScript (TypeScript later) |
| Build | Vite |
| UI | React |
| Styling | Tailwind CSS |
| Routing | React Router |
| Quality | ESLint + Prettier |
| Deploy | Netlify |
| Version control | Git + GitHub |
