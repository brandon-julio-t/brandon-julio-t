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

I lead and build software for messy real-world workflows: ERP platforms, financial operations,
inventory systems, AI-assisted operations, internal tools, and customer-facing portals. I care about
fast iteration, clean product behavior, data correctness, and production systems that stay
understandable after they scale.

- 🏗️ Core builder of Farmio's product stack across ERP, backend services, portals, workers,
  deployment, and operational tooling.
- 🧾 Design correctness-first database flows, including `SERIALIZABLE` transaction isolation for
  money, inventory, reconciliation, and other high-integrity workflows.
- 🤖 Led AI product work including an analytics assistant and Chat Order AI Agent, with reported
  productivity gains of 70% for analytics work and 60% for customer service workflows.
- 🔭 Own production hardening across health checks, observability, OpenTelemetry tracing, deploy
  scripts, and operator documentation.
- 📄 Build business-critical document systems including invoice PDFs, credit-note workflows, font
  rendering fixes, retry/timeout handling, and regression coverage.
- 💸 Reduced AWS S3 storage by 48%, translating to roughly 50% cost savings.
- 🌍 Contribute upstream fixes to tools I use, including deck.gl, OpenClaw, Effect, Convex, PostHog,
  Pitchfork, Opencode, ghui, Motion Primitives, React docs, and Vague.

---

## 🌍 Open Source Highlights

| Project                                                                                                                                                                                                        | Contribution                                                                                                                                                                                                                                                                                                                                                                                                                 | Status                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="assets/icons/effect.svg" width="20" height="20" alt="">&nbsp; [Effect #8843](https://github.com/Effect-TS/effect/issues/8843) + [#8842](https://github.com/Effect-TS/effect/pull/8842)               | Traced a tool crash to a missing dependency that TypeScript had failed to catch. Reported the bug and contributed the fix so incomplete MCP servers fail type checks before they run.                                                                                                                                                                                                                                        | ✅ Reported & fix merged                                                                                                                          |
| <img src="assets/icons/posthog.png" width="20" height="20" alt="">&nbsp; [PostHog AI #5055](https://github.com/PostHog/posthog-js/issues/5055) + [#5056](https://github.com/PostHog/posthog-js/pull/5056)      | Found cache token counts missing from OpenAI Agents traces in PostHog. Reported the gap and contributed a fix so AI usage reports include cached input.                                                                                                                                                                                                                                                                      | 🚀 Shipped in [`@posthog/ai 8.13.4`](https://github.com/PostHog/posthog-js/releases/tag/%40posthog/ai%408.13.4)                                   |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #161836](https://github.com/openclaw/openclaw/issues/161836) + [#161842](https://github.com/openclaw/openclaw/pull/161842) | Traced disappearing chat images to a lost file reference when OpenClaw moved uploaded files. Reported the bug and contributed a fix so previews survive history reloads without exposing private paths.                                                                                                                                                                                                                      | ✅ Reported & fix merged                                                                                                                          |
| <img src="assets/icons/deck-gl.png" width="20" height="20" alt="">&nbsp; [deck.gl #10723](https://github.com/visgl/deck.gl/issues/10723) + [#10724](https://github.com/visgl/deck.gl/pull/10724)               | Traced misplaced tooltips and widgets to a layout bug in deck.gl's React integration. Reported it with visual reproductions and contributed the fix so they stay aligned with the visualization.                                                                                                                                                                                                                             | ✅ Reported & fix merged                                                                                                                          |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #160889](https://github.com/openclaw/openclaw/issues/160889) + [#160895](https://github.com/openclaw/openclaw/pull/160895) | Found OpenClaw resending conversation history that OpenAI had already compressed. Traced the lost checkpoint, reported the bug, and contributed a fix verified against the live API.                                                                                                                                                                                                                                         | ✅ Reported & fix merged                                                                                                                          |
| <img src="assets/icons/effect.svg" width="20" height="20" alt="">&nbsp; [Effect #7015](https://github.com/Effect-TS/effect/issues/7015) + [#7016](https://github.com/Effect-TS/effect/pull/7016)               | Traced failed production retries to timer storage that rejected fractional milliseconds. Reported the bug and contributed a fix so retries are scheduled without shortening the delay.                                                                                                                                                                                                                                       | ✅ Reported & fix merged                                                                                                                          |
| <img src="assets/icons/pitchfork.png" width="20" height="20" alt="">&nbsp; [Pitchfork #580](https://github.com/jdx/pitchfork/pull/580)                                                                         | Traced Pitchfork's failure on Amazon Linux ARM64 to a release build requiring a newer system library. Contributed a fix that pins the build environment, then verified it on Amazon Linux 2023.                                                                                                                                                                                                                              | ✅ Merged                                                                                                                                         |
| <img src="assets/icons/convex.png" width="20" height="20" alt="">&nbsp; [Convex Agent #190](https://github.com/get-convex/agent/issues/190)                                                                    | Traced severe chat lag to long, streamed tool inputs. Reported the bug and supplied a [prototype fix](https://gist.github.com/brandon-julio-t/b203784e2421b35dd7bf7e427483919e) and [benchmark reproduction](https://github.com/brandon-julio-t/agent-190-repro) before maintainers merged the upstream fix.                                                                                                                 | ✅ Upstream fix merged in [#270](https://github.com/get-convex/agent/pull/270)                                                                    |
| 🖥️ [ghui](https://github.com/kitlangton/ghui/compare/v0.4.3...v0.4.4)                                                                                                                                          | Contributed [the Vague theme](https://github.com/kitlangton/ghui/pull/7) and [wraparound keyboard navigation](https://github.com/kitlangton/ghui/pull/8) for the theme picker. Maintainers shipped both changes in `v0.4.4` ([theme](https://github.com/kitlangton/ghui/commit/8e357eeffc3bff6870553a90a5cdb137567c0a61), [navigation](https://github.com/kitlangton/ghui/commit/5c5576db79928e0102166b04cd312d16831ad2c8)). | 🚀 Shipped in [`v0.4.4`](https://github.com/kitlangton/ghui/releases/tag/v0.4.4)                                                                  |
| <img src="assets/icons/posthog.png" width="20" height="20" alt="">&nbsp; [PostHog #54002](https://github.com/PostHog/posthog/pull/54002)                                                                       | Traced AI requests appearing under anonymous IDs in PostHog to discarded user and session data. Contributed the fix so Vercel AI activity stays linked to the correct user and session.                                                                                                                                                                                                                                      | ✅ Merged                                                                                                                                         |
| <img src="assets/icons/convex.png" width="20" height="20" alt="">&nbsp; [Convex #441](https://github.com/get-convex/convex-backend/issues/441) + [#442](https://github.com/get-convex/convex-backend/pull/442) | Found Next.js still running after stopping Convex with `Ctrl+C` through `bun run`. Reported the shutdown bug and proposed a fix so both development servers stop together.                                                                                                                                                                                                                                                   | 🛠️ Shipped in the [`convex v1.36.0` changelog](https://github.com/get-convex/convex-backend/blob/main/npm-packages/convex/CHANGELOG.md#L257-L269) |
| <img src="assets/icons/vague.png" width="20" height="20" alt="">&nbsp; [Vague #8](https://github.com/vague-theme/vague/issues/8) + [#12](https://github.com/vague-theme/vague/issues/12)                       | Built Vague themes for [OpenCode](https://github.com/vague-theme/vague-opencode) and [bat](https://github.com/vague-theme/vague-bat), then transferred both projects to the Vague organization. The bat theme also works with `delta` and `lazygit`.                                                                                                                                                                         | 🎨 Transferred                                                                                                                                    |
| <img src="assets/icons/opencode.png" width="20" height="20" alt="">&nbsp; [OpenCode #13720](https://github.com/anomalyco/opencode/pull/13720)                                                                  | OpenCode's font picker did not include GeistMono Nerd Font. Added the font option across settings and translations.                                                                                                                                                                                                                                                                                                          | ✅ Merged                                                                                                                                         |
| <img src="assets/icons/motion-primitives.svg" width="20" height="20" alt="">&nbsp; [Motion Primitives #146](https://github.com/ibelick/motion-primitives/pull/146)                                             | Found that installing some animation components through shadcn omitted a required package. Fixed the component registry so `react-use-measure` installs automatically.                                                                                                                                                                                                                                                       | ✅ Merged                                                                                                                                         |
| <img src="assets/icons/react.png" width="20" height="20" alt="">&nbsp; [React (Indonesian) #472](https://github.com/reactjs/id.react.dev/pull/472)                                                             | Contributed the first Indonesian translation of React's "Updating Objects in State" guide so readers can learn it in their language.                                                                                                                                                                                                                                                                                         | ✅ Merged                                                                                                                                         |

---

## 🧩 Product Work

| Area                     | Work                                                                                                                                   |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| 🏭 Farmio ERP            | Technical ownership across order management, invoicing, payment reconciliation, inventory control, driver tasking, and route planning. |
| 🤖 AI workflows          | Analytics assistant for business data exploration and Chat Order AI Agent for customer service operations.                             |
| 🧾 Database correctness  | Serializable transaction boundaries for financial and inventory workflows where consistency matters more than theoretical throughput.  |
| 💸 Cost optimization     | AWS S3 storage cleanup that cut stored data by 48%.                                                                                    |
| ✨ UI engineering        | Animated components, dashboard surfaces, mobile-first workflows, and shadcn/Tailwind systems.                                          |
| ⚙️ Engineering systems   | Deployment, health checks, observability, dependency maintenance, production docs, and technical standards.                            |
| 🛠️ Open-source ecosystem | Practical upstream fixes across deck.gl, OpenClaw, Effect, PostHog, Opencode, Convex, and Motion Primitives.                           |

---

## 💼 Experience

| Role               | Company                                          | Period         |
| ------------------ | ------------------------------------------------ | -------------- |
| Tech Lead          | [Farmio](https://farmio.io)                      | 2024 - Present |
| Fullstack Engineer | [BINUS University](https://binus.ac.id) R&D Team | 2020 - 2023    |
| Teaching Assistant | [BINUS University](https://binus.ac.id)          | 2020 - 2021    |

---

## 🛠️ Operating Range

- 🎨 **Frontend:** React, Next.js, TypeScript, Tailwind CSS, shadcn/ui, motion-heavy interfaces
- 🧱 **Backend:** Node.js, Express, PostgreSQL, Redis, Prisma, transaction isolation, API design,
  background workflows
- 🤖 **AI/LLM:** AI agents, chat apps, RAG patterns, OpenAI integrations, LLM analytics
- ☁️ **Infra:** AWS, Docker, Vercel, CI/CD, cost optimization
- 🧪 **Other:** Python, Go, PHP, Solidity, Ethereum

---

## ✨ Selected Projects

- 🎛️ [Animated components](https://brandonjuliothenaro.my.id/components) - web animation experiments
  and UI component work.
- 💬 [T3 Chat Clone](https://github.com/brandon-julio-t/t3-chat-clone) - LLM chat UI cloneathon
  across modern chat product patterns.
- 🧾 [Mini Invoice](https://github.com/brandon-julio-t/mini-invoice) - mobile invoicing app built
  for a real family workflow.
- ⚡ [Slack Clone](https://github.com/brandon-julio-t/slack-clone) - real-time collaboration app
  exploring Slack-style product behavior.
- ⛓️
  [Web3 Event Management](https://github.com/brandon-julio-t/decentralized-event-membership-management) -
  Solidity and Hardhat dApp for decentralized event membership.

---

## 📜 Certifications

- ☁️ AWS Certified Cloud Practitioner
- ⛓️ Ethereum Developer Bootcamp, Alchemy University
- ✨ Animations on the Web, Emil Kowalski
- 🧩 freeCodeCamp: JavaScript Algorithms, Front End Libraries, APIs & Microservices

---

<div align="center">

**Good software earns trust by making the next action obvious.**

📫 Hit me up on [LinkedIn](https://www.linkedin.com/in/brandonjuliothenaro/) ·
[X / Twitter](https://twitter.com/brandon_julio_t) ·
[Instagram](https://www.instagram.com/brandon.julio.t/)

</div>
