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

| Project                                                                                                                                                                                                        | Contribution                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Status                                                                                                                                                             |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #172007](https://github.com/openclaw/openclaw/issues/172007) + [#172016](https://github.com/openclaw/openclaw/pull/172016) | Zooming into screenshots in OpenClaw could send the image drifting offscreen. Reported the bug and contributed the fix so users can inspect image details while keeping the point under the cursor in place.                                                                                                                                                                                                                                                                                                     | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #179331](https://github.com/openclaw/openclaw/issues/179331) + [#179333](https://github.com/openclaw/openclaw/pull/179333) | Concurrent OpenClaw automations could reject the same saved account before any work began, even though its credentials had not changed. Reported the race and contributed the fix so scheduled runs can share an unchanged account while still refusing replaced or revoked credentials.                                                                                                                                                                                                                         | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #180308](https://github.com/openclaw/openclaw/issues/180308) + [#180321](https://github.com/openclaw/openclaw/pull/180321) | Routine inspection of OpenClaw’s AI tool connections printed usable credentials into terminal output and retained agent transcripts. Reported the exposure and contributed credential redaction so operators can inspect connections without revealing supported secret fields or losing saved credentials when editing the output.                                                                                                                                                                              | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #172174](https://github.com/openclaw/openclaw/issues/172174) + [#172176](https://github.com/openclaw/openclaw/pull/172176) | OpenClaw’s automation editor left a visible gap below its Create, Save, and Cancel actions. Reported the layout bug and contributed the fix so the actions sit at the bottom edge on desktop and mobile while remaining reachable by keyboard.                                                                                                                                                                                                                                                                   | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/pkgx.png" width="20" height="20" alt="">&nbsp; [pkgx Pantry #14808](https://github.com/pkgxdev/pantry/pull/14808)                                                                       | OAuth2 Proxy packages still used a Go runtime that trusted compromised certificate authorities. Contributed a build requirement for Go’s certificate protection and verified that a rebuilt package rejects the affected chains. Maintainers rebuilt the latest packages so pkgx users receive that protection too.                                                                                                                                                                                              | ✅ Merged                                                                                                                                                          |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #151374](https://github.com/openclaw/openclaw/issues/151374) + [#151375](https://github.com/openclaw/openclaw/pull/151375) | Chinese and single-word audio transcripts appeared as blank chat bubbles in OpenClaw. Reported the rendering bug and contributed the fix so users can read both new and saved transcripts without migrating their chat history.                                                                                                                                                                                                                                                                                  | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/effect.svg" width="20" height="20" alt="">&nbsp; [Effect #6830](https://github.com/Effect-TS/effect/issues/6830) + [#6832](https://github.com/Effect-TS/effect/pull/6832)               | Effect’s OpenAI integration left developers unable to configure supported cache settings and safety identifiers through its high-level API. Documented the missing request options and proposed a fix; upstream contributors completed the support so applications can configure cache reuse and identify end users for safety monitoring.                                                                                                                                                                       | ✅ Reported & proposed fix; resolved upstream in [#7403](https://github.com/Effect-TS/effect/pull/7403) and [#9670](https://github.com/Effect-TS/effect/pull/9670) |
| <img src="assets/icons/effect.svg" width="20" height="20" alt="">&nbsp; [Effect #6831](https://github.com/Effect-TS/effect/issues/6831) + [#6833](https://github.com/Effect-TS/effect/pull/6833)               | Stable instructions and documents could not be marked for OpenAI cache reuse through Effect’s prompt API. Reported the gap and proposed content-level cache breakpoints; upstream contributors added support for text, images, and files so developers can choose the reusable prefix before changing content.                                                                                                                                                                                                   | ✅ Reported & proposed fix; resolved upstream in [#7403](https://github.com/Effect-TS/effect/pull/7403) and [#9667](https://github.com/Effect-TS/effect/pull/9667) |
| <img src="assets/icons/pkgx.png" width="20" height="20" alt="">&nbsp; [pkgx Pantry #14531](https://github.com/pkgxdev/pantry/pull/14531)                                                                       | The latest pkgx package for OAuth2 Proxy, used to protect web apps behind a login, was missing Go security and reliability fixes included in the official release. Contributed the build fix so pkgx users receive those patches too.                                                                                                                                                                                                                                                                            | ✅ Merged                                                                                                                                                          |
| <img src="assets/icons/effect.svg" width="20" height="20" alt="">&nbsp; [Effect #8843](https://github.com/Effect-TS/effect/issues/8843) + [#8842](https://github.com/Effect-TS/effect/pull/8842)               | An AI tool server could pass TypeScript checks yet crash because a required dependency was missing. Traced the gap in Effect's type checks and contributed the fix so developers catch the mistake before running their tools.                                                                                                                                                                                                                                                                                   | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/posthog.png" width="20" height="20" alt="">&nbsp; [PostHog AI #5055](https://github.com/PostHog/posthog-js/issues/5055) + [#5056](https://github.com/PostHog/posthog-js/pull/5056)      | PostHog's OpenAI Agents reports left out cached token usage, hiding how much input was reused. Reported the gap and contributed the fix so teams can distinguish cached input from fresh input when reviewing AI usage and costs.                                                                                                                                                                                                                                                                                | 🚀 Shipped in [`@posthog/ai 8.13.4`](https://github.com/PostHog/posthog-js/releases/tag/%40posthog/ai%408.13.4)                                                    |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #161836](https://github.com/openclaw/openclaw/issues/161836) + [#161842](https://github.com/openclaw/openclaw/pull/161842) | Reopening an OpenClaw chat made uploaded images disappear. Traced the problem to files being moved and contributed the fix so new uploads remain visible after reloads while private file paths stay hidden.                                                                                                                                                                                                                                                                                                     | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/deck-gl.png" width="20" height="20" alt="">&nbsp; [deck.gl #10723](https://github.com/visgl/deck.gl/issues/10723) + [#10724](https://github.com/visgl/deck.gl/pull/10724)               | Tracked misplaced hover details and controls in deck.gl's React maps to a layout bug that put them below the visualization or offscreen. Reported it with visual reproductions and contributed the fix so users see details beside the point they are exploring.                                                                                                                                                                                                                                                 | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/openclaw.png" width="20" height="20" alt="">&nbsp; [OpenClaw #160889](https://github.com/openclaw/openclaw/issues/160889) + [#160895](https://github.com/openclaw/openclaw/pull/160895) | OpenClaw kept resending old conversation history even after OpenAI had compressed it. Traced the lost compression state and contributed the fix so later AI tool calls keep the compacted history instead of needlessly resending the full conversation.                                                                                                                                                                                                                                                         | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/effect.svg" width="20" height="20" alt="">&nbsp; [Effect #7015](https://github.com/Effect-TS/effect/issues/7015) + [#7016](https://github.com/Effect-TS/effect/pull/7016)               | Investigated Effect workflows that failed before they could retry after an error. Traced the failure to retry delays with fractional milliseconds and contributed the fix so automated retries can be scheduled without firing earlier than requested.                                                                                                                                                                                                                                                           | ✅ Reported & fix merged                                                                                                                                           |
| <img src="assets/icons/pitchfork.png" width="20" height="20" alt="">&nbsp; [Pitchfork #580](https://github.com/jdx/pitchfork/pull/580)                                                                         | Upgrading Pitchfork, a tool for managing background services, broke startup on Amazon Linux ARM64. Traced the failure to its release build and contributed a fix that restores compatibility with existing Linux hosts.                                                                                                                                                                                                                                                                                          | ✅ Merged                                                                                                                                                          |
| <img src="assets/icons/convex.png" width="20" height="20" alt="">&nbsp; [Convex Agent #190](https://github.com/get-convex/agent/issues/190)                                                                    | Convex AI chats slowed to a crawl while an agent streamed a long tool request. Reported the slowdown and supplied a [prototype fix](https://gist.github.com/brandon-julio-t/b203784e2421b35dd7bf7e427483919e) and [benchmark reproduction](https://github.com/brandon-julio-t/agent-190-repro); maintainers later merged a fix to keep chats responsive during tool use.                                                                                                                                         | ✅ Upstream fix merged in [#270](https://github.com/get-convex/agent/pull/270)                                                                                     |
| 🖥️ [ghui](https://github.com/kitlangton/ghui/compare/v0.4.3...v0.4.4)                                                                                                                                          | Brought [the Vague theme](https://github.com/kitlangton/ghui/pull/7) to ghui so users can match their other terminal tools. Also contributed [wraparound keyboard navigation](https://github.com/kitlangton/ghui/pull/8), making the theme picker loop from last to first. Maintainers shipped both in `v0.4.4` ([theme](https://github.com/kitlangton/ghui/commit/8e357eeffc3bff6870553a90a5cdb137567c0a61), [navigation](https://github.com/kitlangton/ghui/commit/5c5576db79928e0102166b04cd312d16831ad2c8)). | 🚀 Shipped in [`v0.4.4`](https://github.com/kitlangton/ghui/releases/tag/v0.4.4)                                                                                   |
| <img src="assets/icons/posthog.png" width="20" height="20" alt="">&nbsp; [PostHog #54002](https://github.com/PostHog/posthog/pull/54002)                                                                       | AI requests appeared under anonymous users in PostHog even though the app supplied user and session IDs. Traced the data loss and contributed the fix so teams can connect AI activity to the correct user and session.                                                                                                                                                                                                                                                                                          | ✅ Merged                                                                                                                                                          |
| <img src="assets/icons/convex.png" width="20" height="20" alt="">&nbsp; [Convex #441](https://github.com/get-convex/convex-backend/issues/441) + [#442](https://github.com/get-convex/convex-backend/pull/442) | Stopping Convex through `bun run` left the Next.js server running in the background. Reported the bug and proposed a fix; the shipped solution stops both servers together, preventing leftover processes from occupying the development port.                                                                                                                                                                                                                                                                   | 🛠️ Shipped in the [`convex v1.36.0` changelog](https://github.com/get-convex/convex-backend/blob/main/npm-packages/convex/CHANGELOG.md#L257-L269)                  |
| <img src="assets/icons/vague.png" width="20" height="20" alt="">&nbsp; [Vague #8](https://github.com/vague-theme/vague/issues/8) + [#12](https://github.com/vague-theme/vague/issues/12)                       | Built Vague themes for [OpenCode](https://github.com/vague-theme/vague-opencode) and [bat](https://github.com/vague-theme/vague-bat) so users can keep the same colors while coding with AI, reading files, and reviewing Git changes through `delta` and `lazygit`. Transferred both projects to the Vague organization.                                                                                                                                                                                        | 🎨 Transferred                                                                                                                                                     |
| <img src="assets/icons/opencode.png" width="20" height="20" alt="">&nbsp; [OpenCode #13720](https://github.com/anomalyco/opencode/pull/13720)                                                                  | GeistMono Nerd Font was bundled with OpenCode but missing from its font picker. Added the missing font option across settings and translations so users can actually select and use it.                                                                                                                                                                                                                                                                                                                          | ✅ Merged                                                                                                                                                          |
| <img src="assets/icons/motion-primitives.svg" width="20" height="20" alt="">&nbsp; [Motion Primitives #146](https://github.com/ibelick/motion-primitives/pull/146)                                             | Installing Motion Primitives animations through shadcn left out a required package, forcing developers to add it themselves. Fixed the component registry so those components install with their dependency included.                                                                                                                                                                                                                                                                                            | ✅ Merged                                                                                                                                                          |
| <img src="assets/icons/react.png" width="20" height="20" alt="">&nbsp; [React (Indonesian) #472](https://github.com/reactjs/id.react.dev/pull/472)                                                             | Contributed the first Indonesian translation of React's "Updating Objects in State" guide, including its examples and explanations. This gives Indonesian-speaking developers a way to learn the pattern in their own language.                                                                                                                                                                                                                                                                                  | ✅ Merged                                                                                                                                                          |

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
