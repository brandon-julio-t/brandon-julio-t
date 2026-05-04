<div align="center">

# Brandon Julio Thenaro

<p>
  <strong>Tech Lead at <a href="https://farmio.io">Farmio</a></strong><br>
  Product-minded engineering lead focused on operational systems, AI workflows, data correctness, and polished web experiences.
</p>

<p>
  <a href="https://brandonjuliothenaro.my.id">Website</a> ·
  <a href="https://www.linkedin.com/in/brandonjuliothenaro/">LinkedIn</a> ·
  <a href="https://twitter.com/brandon_julio_t">X / Twitter</a> ·
  <a href="https://www.instagram.com/brandon.julio.t/">Instagram</a> ·
  <a href="https://raw.githubusercontent.com/brandon-julio-t/curriculum-vitae/refs/heads/main/dist/Brandon_Julio_Thenaro_CV.pdf">CV</a>
</p>

</div>

---

## 🚢 What I Ship

I lead and build software for messy real-world workflows: ERP platforms, financial operations, inventory systems, AI-assisted operations, internal tools, and customer-facing portals. I care about fast iteration, clean product behavior, data correctness, and production systems that stay understandable after they scale.

- 🏗️ Core builder of Farmio's product stack across ERP, backend services, portals, workers, deployment, and operational tooling.
- 🧾 Design correctness-first database flows, including `SERIALIZABLE` transaction isolation for money, inventory, reconciliation, and other high-integrity workflows.
- 🤖 Led AI product work including an analytics assistant and Chat Order AI Agent, with reported productivity gains of 70% for analytics work and 60% for customer service workflows.
- 🔭 Own production hardening across health checks, observability, OpenTelemetry tracing, deploy scripts, and operator documentation.
- 📄 Build business-critical document systems including invoice PDFs, credit-note workflows, font rendering fixes, retry/timeout handling, and regression coverage.
- 💸 Reduced AWS S3 storage by 48%, translating to roughly 50% cost savings.
- 🌍 Contribute upstream fixes to tools I use, including Convex, PostHog, Opencode, ghui, Motion Primitives, React docs, and Vague.

---

## 🌍 Open Source Highlights

| Project | Contribution | Status |
| --- | --- | --- |
| [get-convex/convex-backend#441](https://github.com/get-convex/convex-backend/issues/441) + [#442](https://github.com/get-convex/convex-backend/pull/442) | Reported and proposed a fix for `convex dev --start` cleanup behavior when launched through `bun run`. | 🛠️ Fix landed |
| [PostHog/posthog#54002](https://github.com/PostHog/posthog/pull/54002) | Preserved Vercel AI OTel user, session, and function identifiers so LLM analytics attach to the right user/session. | ✅ Merged |
| [anomalyco/opencode#13720](https://github.com/anomalyco/opencode/pull/13720) | Added GeistMono Nerd Font as a selectable mono font across app settings and locale strings. | ✅ Merged |
| [kitlangton/ghui](https://github.com/kitlangton/ghui/compare/v0.4.3...v0.4.4) | Opened [#7](https://github.com/kitlangton/ghui/pull/7) for the Vague theme and [#8](https://github.com/kitlangton/ghui/pull/8) for picker-modal wraparound navigation; both PRs were closed after the work shipped in `v0.4.4` via upstream commits [`8e357eeffc3bff6870553a90a5cdb137567c0a61`](https://github.com/kitlangton/ghui/commit/8e357eeffc3bff6870553a90a5cdb137567c0a61) and [`5c5576db79928e0102166b04cd312d16831ad2c8`](https://github.com/kitlangton/ghui/commit/5c5576db79928e0102166b04cd312d16831ad2c8). | 🚀 Shipped v0.4.4 |
| [ibelick/motion-primitives#146](https://github.com/ibelick/motion-primitives/pull/146) | Fixed shadcn registry metadata so `react-use-measure` installs automatically for affected components. | ✅ Merged |
| [reactjs/id.react.dev#472](https://github.com/reactjs/id.react.dev/pull/472) | Contributed the initial Indonesian translation for React's "Updating Objects in State" docs page. | ✅ Merged |
| [vague-theme/vague#12](https://github.com/vague-theme/vague/issues/12) | Transferred my [`vague-bat`](https://github.com/vague-theme/vague-bat) theme into the Vague ecosystem for `bat`, `delta`, and `lazygit` users. | 🎨 Transferred |

---

## 🧩 Product Work

| Area | Work |
| --- | --- |
| 🏭 Farmio ERP | Technical ownership across order management, invoicing, payment reconciliation, inventory control, driver tasking, and route planning. |
| 🤖 AI workflows | Analytics assistant for business data exploration and Chat Order AI Agent for customer service operations. |
| 🧾 Database correctness | Serializable transaction boundaries for financial and inventory workflows where consistency matters more than theoretical throughput. |
| 💸 Cost optimization | AWS S3 storage cleanup that cut stored data by 48%. |
| ✨ UI engineering | Animated components, dashboard surfaces, mobile-first workflows, and shadcn/Tailwind systems. |
| ⚙️ Engineering systems | Deployment, health checks, observability, dependency maintenance, production docs, and technical standards. |
| 🛠️ Developer tooling | Practical upstream fixes in AI/devtool ecosystems including PostHog, Opencode, Convex, and Motion Primitives. |

---

## 💼 Experience

| Role | Company | Period |
| --- | --- | --- |
| Tech Lead | [Farmio](https://farmio.io) | 2024 - Present |
| Fullstack Engineer | [BINUS University](https://binus.ac.id) R&D Team | 2020 - 2023 |
| Teaching Assistant | [BINUS University](https://binus.ac.id) | 2020 - 2021 |

---

## 🛠️ Operating Range

- 🎨 **Frontend:** React, Next.js, TypeScript, Tailwind CSS, shadcn/ui, motion-heavy interfaces
- 🧱 **Backend:** Node.js, Express, PostgreSQL, Redis, Prisma, transaction isolation, API design, background workflows
- 🤖 **AI/LLM:** AI agents, chat apps, RAG patterns, OpenAI integrations, LLM analytics
- ☁️ **Infra:** AWS, Docker, Vercel, CI/CD, cost optimization
- 🧪 **Other:** Python, Go, PHP, Solidity, Ethereum

---

## ✨ Selected Projects

- 🎛️ [Animated components](https://brandonjuliothenaro.my.id/components) - web animation experiments and UI component work.
- 💬 [T3 Chat Clone](https://github.com/brandon-julio-t/t3-chat-clone) - LLM chat UI cloneathon across modern chat product patterns.
- 🧾 [Mini Invoice](https://github.com/brandon-julio-t/mini-invoice) - mobile invoicing app built for a real family workflow.
- ⚡ [Slack Clone](https://github.com/brandon-julio-t/slack-clone) - real-time collaboration app exploring Slack-style product behavior.
- ⛓️ [Web3 Event Management](https://github.com/brandon-julio-t/decentralized-event-membership-management) - Solidity and Hardhat dApp for decentralized event membership.

---

## 📜 Certifications

- ☁️ AWS Certified Cloud Practitioner
- ⛓️ Ethereum Developer Bootcamp, Alchemy University
- ✨ Animations on the Web, Emil Kowalski
- 🧩 freeCodeCamp: JavaScript Algorithms, Front End Libraries, APIs & Microservices

---

<div align="center">

**Good software earns trust by making the next action obvious.**

📫 Hit me up on
[LinkedIn](https://www.linkedin.com/in/brandonjuliothenaro/) ·
[X / Twitter](https://twitter.com/brandon_julio_t) ·
[Instagram](https://www.instagram.com/brandon.julio.t/)

</div>
