# Design Engineering

Welcome to **Design Engineering**, a portfolio-style GitHub repository demonstrating the hybrid skills of a design engineer. This repo blends UI/UX design principles with front-end engineering expertise, focusing on tasks like debugging performance bottlenecks in design systems, prototyping interactive components, and exploring emerging CSS specifications and Web APIs from MDN.

## 30-Day Design Engineering Learning Plan
Use this repo as a self-guided, 30-day learning plan to understand what design engineering is, how design engineers collaborate within teams, and how to build core deliverables (prototypes, UI tooling, and system components). Start with the docs below:

- **Start here**: `docs/README.md`
- **Progress tracker**: `docs/plan.md`
- **Weekly guides**: `docs/weeks/`
- **Sources**: `docs/sources.md`

Inspired by roles at companies like Vercel and Ramp, this showcase includes self-initiated projects that fix real-world issues (e.g., browser quirks) or create new opportunities (e.g., leveraging modern specs for innovative UIs). All activities draw from MDN documentation on CSS features like container queries, cascade layers, and Web APIs such as Intersection Observer, ensuring standards-compliant implementations.

The repo features code examples, interactive demos (hostable via GitHub Pages or Vercel), detailed explanations, and blog-style markdown posts. It's designed as a living portfolio to highlight proactive problem-solving and innovation—core to a design engineer's role.

## Getting Started
- **Clone the Repo**: `git clone https://github.com/yourusername/DesignEngineerShowcase.git`
- **Tech Stack**: Built with HTML/CSS/JS, Next.js for demos, Tailwind CSS, Tweakpane for debug panels, and more.
- **Run Demos**: Navigate to `/prototypes` and serve locally (e.g., via `npx serve`).
- **Contribute**: Fork, create issues/pull requests, or add your own MDN-based demos!

## Repository Structure
- **/blog-posts/**: Markdown files with in-depth articles on debugging and implementations, including code snippets, screenshots, and step-by-step guides.
- **/components/**: Reusable design system components built with HTML/CSS/JS (e.g., using Tailwind or vanilla CSS).
- **/prototypes/**: Interactive demos and playgrounds for experimenting with features.
- **/debug-tools/**: Custom scripts or panels for performance analysis (e.g., Tweakpane integrations).
- **/docs/**: API references or spec explorations based on MDN.
- **README.md**: This file—overview with links to activities and features.

## Key Activities and Projects
Each project is outlined below, with ties to MDN specs/Web APIs. These can be explored as separate branches, folders, or issues/pull requests. They represent tasks a design engineer might self-initiate, such as fixing bugs in design systems or prototyping new features.

1. **Debugging CSS Performance Bottlenecks in Design Systems**
   - **Description**: A demo component library (e.g., a grid of cards) exhibiting performance issues like style recalculations during resizing or scrolling. Profiles with Chrome DevTools, identifies culprits (e.g., inefficient font-relative units like `ch` or `ex`), and fixes by switching to alternatives like `rem`. Includes a blog post with before/after flame charts.
   - **Rationale**: Maintains scalable design systems where CSS choices impact performance in large UIs.
   - **Based on MDN Specs/Web APIs**: CSS Units guide (font-relative vs. viewport units) and Resize Observer API for detecting changes without reflows. Integrates Intersection Observer for lazy-loading to reduce paint times.
   - **Output**: Debug panel with Tweakpane v4.0.5 to toggle units and monitor FPS. See `/blog-posts/css-performance.md` and `/prototypes/perf-bottleneck`.

2. **Implementing Responsive Components with Container Queries**
   - **Description**: Adaptive UI components (e.g., nav bars or modals) that adjust based on container size. Prototypes variations, debugs nested queries, and documents integration into design systems.
   - **Rationale**: Enables modular, "plug-and-play" components without media query overload—perfect for dynamic dashboards.
   - **Based on MDN Specs/Web APIs**: CSS Container Queries (`@container`) and Resize Observer for dynamic styling. Explores style queries for conditional parent-based styles.
   - **Output**: Interactive playground with Figma-linked code and A/B performance tests. See `/blog-posts/container-queries.md` and `/components/responsive-nav`.

3. **Optimizing Cascade and Specificity with Layers**
   - **Description**: Refactors design system CSS using cascade layers to fix overriding conflicts (e.g., in third-party integrations). Includes a visualization tool and migration guide.
   - **Rationale**: Streamlines collaborative CSS architecture, reducing specificity bugs.
   - **Based on MDN Specs/Web APIs**: `@layer` at-rule for organizing layers (base, components, utilities). Pairs with Mutation Observer for dynamic DOM monitoring.
   - **Output**: Layered CSS boilerplate and Tweakpane panel to switch layers. See `/blog-posts/cascade-layers.md` and `/debug-tools/layer-visualizer`.

4. **Creating Interactive Animations with Scroll-Driven Effects**
   - **Description**: Parallax or progress indicators tied to scroll. Debugs jank, optimizes with GPU, and polyfills for browsers.
   - **Rationale**: Adds delight to marketing sites or product UIs.
   - **Based on MDN Specs/Web APIs**: Scroll-driven Animations (`@scroll-timeline`) and Intersection Observer for view-based triggering.
   - **Output**: Demo with scroll analytics and adjustable timelines. See `/blog-posts/scroll-animations.md` and `/prototypes/parallax-demo`.

5. **Exploring Color Manipulation for Theming in Design Systems**
   - **Description**: Theming engine for dynamic palettes, fixing accessibility issues like contrast. Includes dark mode toggles.
   - **Rationale**: Supports rapid branding iterations with customizable UIs.
   - **Based on MDN Specs/Web APIs**: `color-mix()` and relative color syntax for blending. Uses `prefers-color-scheme` media query.
   - **Output**: Color picker with live previews, debugged cross-browser. See `/blog-posts/color-theming.md` and `/components/theme-engine`.

6. **Building Accessible Grids with Subgrid**
   - **Description**: Responsive tables/layouts using subgrid for alignment. Debugs nested issues and integrates design tokens.
   - **Rationale**: Ensures consistency in complex UIs like data dashboards.
   - **Based on MDN Specs/Web APIs**: CSS Grid `subgrid` for track inheritance and Resize Observer for adaptive spans.
   - **Output**: Grid playground with ARIA and performance profiles. See `/blog-posts/subgrid.md` and `/components/accessible-grid`.

7. **Prototyping View Transitions for Smooth Page Changes**
   - **Description**: Seamless animations in SPAs. Debugs glitches and optimizes for mobile.
   - **Rationale**: Polishes navigation flows for engaging experiences.
   - **Based on MDN Specs/Web APIs**: View Transitions API for declarative DOM change animations.
   - **Output**: Demo app with Tweakpane for transition controls. See `/blog-posts/view-transitions.md` and `/prototypes/spa-transitions`.

## Additional Repo Features
- **CI/CD Integration**: GitHub Actions runs Lighthouse audits on pushes to enforce performance standards.
- **Collaboration Hooks**: Open issues for community contributions, like adding MDN-based demos.
- **Metrics Tracking**: Badges for code coverage and perf scores.
- **Inspiration Sources**: Links to MDN docs and company blogs (e.g., Vercel's design engineering posts).

[![License: PolyForm Noncommercial 1.0.0](https://img.shields.io/badge/License-PolyForm%20Noncommercial%201.0.0-blue.svg)](https://polyformproject.org/licenses/noncommercial/1.0.0))
Fork this repo, build on it, and showcase your design engineering prowess. Contributions welcome! 🚀

For questions or collaborations, reach out via issues or [your contact info].
