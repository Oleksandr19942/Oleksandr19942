# Hi, I'm Oleksandr Meteliev

**iOS Engineer** building production health & AI mobile products — from architecture and streaming systems to App Store release.

[LinkedIn](https://www.linkedin.com/in/oleksandr-meteliev-b2ab46209/) · [App Store — 2ndOpinions](https://apps.apple.com/us/app/2ndopinions/id6560104742) · [Case study](https://www.startupsoft.com/cases/2nd-opinion/)

---

## What I'm building now

### [2ndOpinions](https://apps.apple.com/us/app/2ndopinions/id6560104742) — AI health companion (iOS 17+)

Consumer health app that helps users prepare for doctor visits, explore health questions, and organize medical context through an AI-powered chat. **Shipped to the App Store** for the U.S. and Canadian market.

I own the **iOS product end-to-end**: architecture, core features, integrations, release pipeline, and post-launch iteration alongside product, backend, and ML teams.

#### What I built on iOS

**AI chat that feels live**  
Designed and implemented a custom streaming layer on top of the **Azure OpenAI Responses API** (SSE). The app streams model output into the UI in real time, runs a **multi-turn tool-calling loop** (7 local tools), and handles rate limits, cancellation, and recovery when streams fail mid-response.

**Context-aware medical conversations**  
The assistant can pull in data the user actually has on the device and in the cloud:

- **Semantic search** across medical records, chat history, files, medications, and Apple Health data  
- **PDF and image attachments** in conversation input  
- **HealthKit** sync across activity, cardiovascular, sleep, nutrition, and mobility metrics  
- **“Explore with AI”** flows that attach selected medical records directly into an active chat  

**Medical records as a first-class product surface**  
Not just chat — a full records workflow: capture, edit, filter, document viewing, and **resilient uploads** to S3 (background tasks, orphaned-job recovery on launch, batch reconciliation, local notifications). Built with a **coordinator**-driven flow and a clear domain/upload split so the feature could grow without turning into a monolith.

**Monetization & platform glue**  
**StoreKit 2** subscriptions with entitlement checks and restore flows. **AWS Amplify** (Cognito, GraphQL, S3) for auth and sync. **Firebase** for push (FCM) and Crashlytics. **Apple Speech** for voice-to-text in chat.

**Clinical summaries (SOAP)**  
SOAP-style note generation, editing, and PDF export — so users can turn conversations and health data into structured summaries they can share with providers.

**Scale & quality bar**  
The codebase is organized as **23 feature modules** with MVVM, protocol-oriented services, SwiftData caching, and centralized wiring through `AppContainer`. Test coverage includes **31 XCTest suites (400+ tests)** around chat streaming, upload recovery, ViewModels, and HealthKit-related flows.

#### Stack (iOS)

`Swift` `SwiftUI` `async/await` `Combine` `SwiftData` `HealthKit` `StoreKit 2` `PDFKit`  
`AWS Amplify` `GraphQL` `Firebase` `Azure OpenAI` `SSE` `CryptoKit`

---

## Other shipped apps I've worked on

| App | What it is |
|-----|------------|
| [EZLogz](https://apps.apple.com/us/app/ezlogz-eld-truck-navigation/id1171472456) | Fleet & logistics — cargo tracking, ELD/navigation |
| [EzChatAI](https://apps.apple.com/us/app/ezchatai-logistics-ai-chatbot/id6467775442) | AI assistant for drivers — routes, scheduling, cargo context |
| [RomDomDom](https://apps.apple.com/ua/app/romdomdom/id1541853396) | Driving school — client + instructor apps, payments, documents |
| [Momenzo](https://apps.apple.com/us/app/momenzo-the-listing-video-app/id1465399598) | Template-based video creation & sharing (SwiftUI) |
| **P2B** | Crypto exchange — real-time order book & portfolio over **WebSockets**, reusable Swift Package client |

---

## How I work

- **Product-minded engineering** — I care about release quality, edge cases (background uploads, stream recovery, account switching), and what users see in production.  
- **Modular architecture** — features own their UI and domain; shared infrastructure stays in services.  
- **Honest scope** — I describe what I implemented on iOS; backend ML/agent orchestration is collaborative, not “I did everything.”

---

## Background

**4+ years** shipping iOS apps across health-tech, fintech, and logistics.  
**Education:** Lviv Polytechnic National University — Metrology & Information-Measuring Engineering.

**Languages:** English (B2) · Ukrainian (native)

---

*Most production source lives in private repositories. Happy to walk through architecture or specific technical decisions.*
