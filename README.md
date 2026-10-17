<div align="center">

# Hi, I'm Sachin 👋

**Just a curious fellow — building open-source software you can run on your own servers.**

I maintain [**Casual Office**](https://github.com/CasualOffice), an open-source office suite for
self-hosters, and the Rust engines underneath it.

[casualoffice.org](https://casualoffice.org) · [GitHub org](https://github.com/CasualOffice)

</div>

---

## Casual Office

An office suite you deploy yourself: real-time co-editing, `.xlsx` / `.docx` / `.pptx`
round-trip, no vendor lock-in.

### The apps

| Project | What it is | Try it |
| --- | --- | --- |
| [**sheets**](https://github.com/CasualOffice/sheets) | Casual Sheets — self-hosted web spreadsheet with `.xlsx` round-trip and real-time co-editing | [sheet.casualoffice.org](http://sheet.casualoffice.org/) |
| [**docs**](https://github.com/CasualOffice/docs) | Casual Docs — self-hosted web `.docx` editor with real-time co-editing | [docs.casualoffice.org](http://docs.casualoffice.org/) |
| [**slides**](https://github.com/CasualOffice/slides) | Casual Slides — web slides editor with `.pptx` round-trip (paused while Docs and PDF reach v1) | — |
| [**pdf**](https://github.com/CasualOffice/pdf) | Casual PDF — PDF viewer and editor: annotate, forms, in-place text edits, e-signing, co-editing | [pdf.casualoffice.org](https://pdf.casualoffice.org/) |
| [**desktop**](https://github.com/CasualOffice/desktop) | Casual Desktop — private, local-only desktop office suite for Word and Excel files (Tauri + Rust) | [download](https://casualoffice.org/casual-desktop/) |
| [**RASystem**](https://github.com/CasualOffice/RASystem) | Casual RAS — the remote-access engine you embed: consent-first P2P screen sharing in Rust over iroh/QUIC | [ras.casualoffice.org](https://ras.casualoffice.org/) |

### The engines (Rust → WebAssembly)

| Project | What it is | Try it |
| --- | --- | --- |
| [**opencalc**](https://github.com/CasualOffice/opencalc) | OpenCalc — an Excel-compatible spreadsheet engine for `.xlsx`, `.xlsm` and `.ods`, with an editor in WebAssembly | [calc.casualoffice.org](https://calc.casualoffice.org) |
| [**opendoc**](https://github.com/CasualOffice/opendoc) | OpenDoc — embeddable, local-first Word-document engine and editor: DOCX/ODT in, PDF/HTML/Markdown out | [opendoc.casualoffice.org](http://opendoc.casualoffice.org/) |
| [**core**](https://github.com/CasualOffice/core) | A pure-Rust engine that reads, writes and converts DOCX, ODT, PDF, Markdown and text, with WASM and C FFI bindings | [docs](https://casualoffice.github.io/core/) |

### Platform and work tools

| Project | What it is | Try it |
| --- | --- | --- |
| [**enclave**](https://github.com/CasualOffice/enclave) | Enclave — self-hostable enterprise shared workspace: content, permissions, governance, search and AI behind one policy boundary (in development) | — |
| [**doc-hub**](https://github.com/CasualOffice/doc-hub) | Self-hosted document hub — an encrypted, tamper-evident registry for documents your team can't afford to lose or leak | [doc-hub.casualoffice.org](http://doc-hub.casualoffice.org/) |
| [**TaskForge**](https://github.com/CasualOffice/TaskForge) | Self-hostable work tracker in Rust with explainable permissions and configurable workflows | [taskforge.casualoffice.org](https://taskforge.casualoffice.org/) |
| [**Procera**](https://github.com/CasualOffice/Procera) | Open-source business process management: model, automate, govern and improve workflows | [procera.casualoffice.org](http://procera.casualoffice.org/) |
| [**assaybank**](https://github.com/CasualOffice/assaybank) | Self-hosted technical hiring: async assessments, live coding interviews and proctored exams over one question bank (in active build) | — |

### Local-first

| Project | What it is | Try it |
| --- | --- | --- |
| [**marrow**](https://github.com/CasualOffice/marrow) | A local knowledge runtime: indexes folders you grant it and answers with citations to the exact page, cell or line | [docs](https://casualoffice.github.io/marrow/) |
| [**studio**](https://github.com/CasualOffice/studio) | Image models that run entirely on your Mac — generate, edit, upscale, illustrate a story; offline, encrypted at rest | [studio.casualoffice.org](https://studio.casualoffice.org/) |

### Shared infrastructure

| Project | What it is |
| --- | --- |
| [**collab**](https://github.com/CasualOffice/collab) | Real-time collaboration server for the self-hosted editors — Hocuspocus + Yjs with auth, WOPI, storage, snapshots and versioning |
| [**univer-revamp**](https://github.com/CasualOffice/univer-revamp) | Fork of the Univer spreadsheet framework carrying the patches Casual Sheets depends on |
| [**website**](https://github.com/CasualOffice/website) | [casualoffice.org](https://casualoffice.org/) |

---

## Also building

| Project | What it is |
| --- | --- |
| [**FigCraft Cloud**](https://github.com/schnsrw/figcraft) | Self-hostable, browser-based collaborative interface design in pure Rust: real-time co-editing, durable PostgreSQL/S3 storage, multi-tenancy, OIDC/SAML. A fork of [FigCraft](https://github.com/storytold/figcraft) — [site](https://schnsrw.github.io/figcraft/) · [try the editor](https://schnsrw.github.io/figcraft/edit/) |
| [**transcribe**](https://github.com/schnsrw/transcribe) | Lightweight, multilingual, low-hallucination live-call transcription with a Jigasi-compatible WebSocket wire format and pluggable ASR backends |
| [**file.sync**](https://github.com/schnsrw/file.sync) | File synchronisation (Java) |

---

## How I build

**Rust** for engines and servers (Axum, SQLx, PostgreSQL), compiled to **WebAssembly** when the
engine has to run in a browser tab · **TypeScript / React** for web editors · **Tauri** for
desktop · Docker Compose so every product self-hosts.

Things I care about: files stay in their real format, nothing is lost silently, and you can run
all of it yourself.

Contributions are welcome on any of these — open an issue or a PR.
