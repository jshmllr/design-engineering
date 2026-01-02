# Learning Path (Self-Paced)

This is a practical path to become a design engineer by repeatedly cycling through:

**Learn → Rebuild → Systematize → Polish → Ship → Reflect**

Use the templates in `templates/` to track progress.

## 0) Orientation (half-day)

- Read:
  - `https://vercel.com/blog/design-engineering-at-vercel`
  - `https://adobe.design/stories/leading-design/should-you-pursue-a-career-in-design-engineering`
  - `https://www.designengineer.xyz/design-engineering`
- Write:
  - Your own definition of design engineering (3–5 sentences)
  - The kind of work you want to do (marketing UI, product UI, design systems, motion, etc.)
- Output:
  - A study log entry using `templates/study-log.md`

## 1) Web foundations (Week 1–2)

- **HTML**: semantics, forms, responsive images, document structure
- **CSS**: layout (flex/grid), sizing, typography, responsive design
- **JS**: DOM, events, state, async basics

Recommended reference:

- `https://developer.mozilla.org/en-US/`

Outputs:

- Rebuild 2–3 common UI patterns in pure HTML/CSS:
  - header/nav
  - card list
  - form
- Add baseline a11y:
  - focus states
  - labels
  - keyboard navigation

## 2) CSS craft (Week 3–4)

Focus on the details that make interfaces feel “designed”, not merely “functional”.

- Layout rhythm, spacing systems
- Typography: scale, line-length, optical alignment
- Interaction states and micro-interactions
- Motion fundamentals (duration/easing, reducing motion)

Primary learning:

- `https://www.joshwcomeau.com/css/`
- `https://css-tricks.com/`
- MDN CSS reference: `https://developer.mozilla.org/en-US/docs/Web/CSS`

Outputs:

- Create a component “gallery” page: buttons, inputs, menus, tooltips, dialogs
- Add a motion pass:
  - hover/press states
  - enter/exit transitions where appropriate

## 3) Design systems mindset (Week 5–7)

Learn to build UI that can scale across a product: tokens, constraints, patterns, guidelines.

Study:

- Vercel guidelines as a real-world reference system: `https://vercel.com/design/guidelines`

Outputs:

- Define tokens (even if in JSON/CSS variables):
  - color, spacing, radii, type scale, shadows
- Create 8–12 components with consistent APIs:
  - Button, Input, Select, Checkbox, Tabs, Badge, Toast, Modal, Tooltip, Card, Table
- Write usage guidelines:
  - when to use, when not to use, accessibility notes, content guidelines

## 4) Quality bar: accessibility + performance (Week 8–9)

Accessibility:

- Semantic structure, focus management, ARIA only when needed
- Keyboard-first interactions
- Color contrast and motion sensitivity

Performance:

- Reduce layout thrash and expensive effects
- Understand what triggers layout/paint/composite
- Image loading basics (sizes, formats, responsive)

References:

- MDN accessibility: `https://developer.mozilla.org/en-US/docs/Web/Accessibility`
- MDN performance: `https://developer.mozilla.org/en-US/docs/Learn/Performance`

Outputs:

- Audit one of your earlier components/pages:
  - keyboard walkthrough
  - contrast checks
  - perf profiling notes (what you changed and why)

## 5) Tooling fluency (Week 10–11)

The goal isn’t “knowing every tool”—it’s being able to pick the right tool and work quickly.

Browse (curate your own stack):

- `https://www.designengineer.xyz/tools`

Common options to explore:

- Figma (handoff + prototyping)
- Storybook (component documentation)
- React + Next.js (UI development)
- Tailwind or vanilla CSS (tradeoffs)
- Motion (CSS/WAAPI)

Outputs:

- Document your personal toolkit:
  - what you use for design, code, docs, testing, profiling

## 6) Capstone + portfolio narrative (Week 12)

Pick one project from `docs/projects.md` and take it to a “shareable” state:

- README with problem statement and screenshots
- Clear component APIs and guidelines
- A11y + perf notes
- A short write-up: what you learned, what you’d do next

