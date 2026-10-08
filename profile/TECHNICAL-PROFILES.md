# Software engineering profiles

[Portfolio and demonstrations](https://github.com/BrysonCo)

Individual profiles of the software behind this portfolio: what each system does, how it is structured, its implementation footprint, and the evidence available for review. My contribution combines product architecture and direction, AI-assisted implementation, integration, review, testing, and delivery.

Measurements describe the reviewed private source snapshots of **October 8, 2026**. “LOC” means nonblank, non-comment source lines, including interface styles, schema SQL, and operational tooling. Test/support files are counted separately. These are measures of source footprint, not individual authorship, product quality, or completed features. See the [counting method](#counting-method) for exclusions and limits.

## Ownce

**User-owned applications with shared local AI, identity, knowledge, and device integration.** The suite connects application experiences to self-hosted services and open-source engines.

| Engineering dimension | Reviewed source |
|---|---|
| Implementation footprint | **420,464 LOC across 1,933 files** |
| Principal languages | Python, TypeScript, Rust, CSS, Kotlin; JavaScript and operational scripts |
| Structure | Typed Python/FastAPI/Pydantic services; React/TypeScript/Vite hub; Rust/Tauri clients; Matrix SDK bridge; Kotlin Android plugins; shared host contracts |
| Platforms | Web and Windows desktop implementations; native Android implementation; future iOS |
| Test/support source | 988 files, 166,120 LOC; presence is not a passing-test or coverage claim |

The engineering work spans scoped AI tools, media integration, retrieval, native client boundaries, and cross-device workflows. Android has emulator evidence; device qualification and distribution remain separate work. iOS preparation does not establish a delivered iOS application.

The following are **selected embedded application profiles**, not a complete inventory of every Ownce application or component.

### Listen

**Music discovery, library, playlists, and playback.** TypeScript application and player interfaces connect through Python services to Navidrome/Subsonic-compatible music services. The direct application footprint is **12,457 LOC in 26 files**: TypeScript 7,176; CSS 2,858; Python 2,423.

The implementation covers library search, album/artist discovery, queues, favourites, and history. Audible gapless playback and native offline/download qualification remain open verification areas.

### Watch

**Movie and television library and player.** A TypeScript interface and Python integration layer work with Jellyfin. The direct application footprint is **11,853 LOC in 22 files**: TypeScript 6,268; Python 2,852; CSS 2,733.

The implementation includes episode navigation, subtitles, progress/resume, personal lists, history, and playback preferences. The portfolio screenshot demonstrates browsing with sample data. Download and casting features are not claimed.

### Maps

**Maps, place search, routes, and guidance.** MapLibre interfaces use Python service integrations with Photon and Valhalla. The direct application footprint is **6,557 LOC in 22 files**: TypeScript 2,762; Python 2,377; CSS 1,418.

Saved places, route alternatives, and downloadable map-tile areas are implemented. Tile packs do not provide complete offline routing or offline place search.

### Chat

**Encrypted communication with controlled AI participation.** Native Rust Matrix SDK integration connects application interfaces and native bridges to Matrix services. The direct application footprint is **20,884 LOC in 68 files**: Rust 16,597; TypeScript 2,056; Kotlin 1,096; Python 944; CSS 191.

Source includes attachments, verification/recovery foundations, durable sending, and AI participation controls. Live relay/message acceptance and device qualification remain verification boundaries; client calling is not delivered. Inline Rust tests remain included in this whole-file source count.

### Network

**Infrastructure visibility and supervised maintenance.** A TypeScript interface and Python Omada integration support device/client views, topology, WAN history, incidents, alerts, and confirmation-based maintenance foundations. The direct application footprint is **13,071 LOC in 46 files**: TypeScript 6,066; Python 4,177; CSS 2,828.

Shared gateway integration and hardware acceptance remain active work.

### Knowledge & Library

**An owned reference collection and retrieval system.** Python extraction, indexing, hybrid retrieval, reranking, ZIM handling, provenance, and research-dossier modules connect to TypeScript interfaces. The direct application footprint is **13,813 LOC in 68 files**: Python 13,053; TypeScript 760.

These modules include editable knowledge and evaluation work. The full notebook-style research workflow remains under development. The demonstrated Notebook editor and CAD sketcher are implemented components, not proof of that complete research workflow.

**Application-count boundary:** These six footprints are explicit source-path subsets already included in Ownce's overall count. They exclude shared gateway, identity, memory, voice, shell, and device services, so they are not the full engineering size of each application. Open-source service dependencies are not counted as Ownce implementation.

## Project Operations

**Project planning, delivery workflows, business records, and document access.**

| Engineering dimension | Reviewed source |
|---|---|
| Implementation footprint | **270,467 LOC across 1,559 files** |
| Principal languages | TypeScript 145,469 LOC; C# 115,208; JavaScript, Bicep, SQL, and supporting source |
| Structure | ASP.NET Core/.NET 8 API and Azure Functions; Entity Framework/SQL Server; Next.js/React interface; Electron desktop; Outlook/Teams surfaces; TypeScript MCP package |
| Platforms | Browser and Windows desktop source with Microsoft integrations |
| Test/support source | 107 files, 26,504 LOC |

The structure separates service logic, persistence, user interfaces, and integrations. Generated schema migrations and bundled add-in assets are excluded from the reported footprint. Cross-platform build declarations are not evidence of qualified macOS/Linux releases. This profile is based on local source inspection, not a fresh cloud deployment validation.

## IoT Control Interface

**Device monitoring, administration, telemetry handling, and archival tools.**

| Engineering dimension | Reviewed source |
|---|---|
| Implementation footprint | **23,375 LOC across 150 files** |
| Principal languages | TypeScript 15,009 LOC; Dart 6,593; JavaScript 1,606; Kotlin and supporting source |
| Structure | React/TypeScript/Vite client; Express/Node service; Azure Functions; Cosmos and IoT Hub integrations; Dart/Flutter mobile source |
| Platforms | Browser dashboard and mobile implementation source |
| Test/support source | 1 file, 9 LOC |

The source separates the dashboard, API/service functions, telemetry integrations, and mobile client. Flutter platform scaffolding is not evidence of qualified platform releases. Automated test evidence in this reviewed snapshot is limited; this profile does not claim production qualification.

## Archivist

**Local archive and media organization with reviewable, reversible workflows.**

| Engineering dimension | Reviewed source |
|---|---|
| Implementation footprint | **88,245 LOC across 273 files** |
| Principal languages | Python 47,948 LOC; TypeScript 33,766; CSS 5,278; SQL and Rust |
| Structure | Python media-analysis engine and FastAPI service; React/TypeScript/Vite interface; Rust/Tauri native shell |
| Platforms | Windows desktop and webview interface |
| Test/support source | 142 files, 27,645 LOC |

The architecture separates analysis and background work from the desktop interface and native shell. The portfolio includes an actual drive/folder-selection capture. Approval-before-move is part of the workflow; the screenshot does not imply that every proposed organization branch is complete.

## Personal knowledge engine

**Capture, organization, curation, and recall over a structured knowledge vault.**

| Engineering dimension | Reviewed source |
|---|---|
| Implementation footprint | **10,851 LOC across 72 files** |
| Principal languages | TypeScript 9,614 LOC; Python 739; JavaScript 296; PowerShell 202 |
| Structure | Node/TypeScript MCP server; curator and read-side modules; Python/PowerShell operational helpers; Node test tooling |
| Platforms | Local service and command-line tools used through AI tool interfaces |
| Test/support source | 10 files, 1,250 LOC |

The software keeps the knowledge vault separate from the engine. Personal vault contents are excluded from both this source snapshot and the public portfolio.

## Job Search Command Center

**Career evidence, opportunities, application preparation, and assisted browser workflows.**

| Engineering dimension | Reviewed source |
|---|---|
| Implementation footprint | **19,436 LOC across 130 files** |
| Principal languages | TypeScript 15,793 LOC; CSS 2,101; JavaScript 1,340; supporting scripts |
| Structure | pnpm monorepo; Electron/React desktop; WXT browser extension; shared contracts, core, and database packages; SQLite; Vitest |
| Platforms | Windows desktop and Chrome/Brave Manifest V3 extension, connected through native messaging |
| Test/support source | 53 files, 4,765 LOC |

The application uses structured evidence and local persistence to support preparation. Final submission remains user-controlled. Personal career records, application data, and credentials are outside the source footprint.

## Additional application and website work

These profiles distinguish integrated application packages, earlier foundations, and website work from independently released products.

### A Different Matter

**Maker-product operations and scheduling.** Python CLI and SQLite schema, joined to a TypeScript/React cockpit through an Ownce host contract.

- **Footprint:** 8,005 implementation LOC in 8 files; 6 test/support files, 869 LOC.
- **Languages:** TypeScript 4,914 LOC; CSS 1,565; Python 1,215; SQL 311.
- **Form:** Headless engine and Ownce-integrated application source. An independent release is not established by this snapshot.

### Plenello

**Supervised commerce orchestration and unit-economics gates.** Python CLI, gate calculations, SQLite schema, and an LLM client, joined to a TypeScript/React cockpit.

- **Footprint:** 4,831 implementation LOC in 12 files; 5 test/support files, 515 LOC.
- **Languages:** TypeScript 3,412 LOC; Python 1,274; SQL 145.
- **Form:** Headless engine and Ownce-integrated application source. Proposed outward actions are separated from approved execution; an independent release is not established here.

### Consolidated Product Works

**Parent commerce and product-work interface.** TypeScript/React company package and CSS, using the host's React runtime and application contract.

- **Footprint:** 3,075 implementation LOC in 8 files; no separately classified test/support files in this export.
- **Languages:** CSS 2,004 LOC; TypeScript 1,071.
- **Form:** Ownce-integrated application source. This profile does not claim a separate deployed service.

### AI Video Factory

**Video/content-production workflows and a review queue.** Python factory and voice-lab modules, FastAPI/MCP dependencies, a React/Vite review interface, and an Ownce-integrated package.

- **Footprint:** 17,358 implementation LOC in 61 files; 1 test/support file, 173 LOC.
- **Languages:** TypeScript 5,800 LOC; Python 5,602; CSS 3,803; JSX 2,044; supporting source.
- **Form:** Headless service and browser-interface source. The snapshot includes preserved legacy cockpit work; an independent deployment is not asserted.

### Wateree Media

**Agency workroom and creative/site-production interfaces.** TypeScript/React application package and CSS with an explicit transitional Ownce host contract.

- **Footprint:** 10,075 implementation LOC in 26 files; no separately classified test/support files in this export.
- **Languages:** TypeScript 7,513 LOC; CSS 2,562.
- **Form:** Ownce-integrated application source, including migration-era interface work. Independent delivery is not established by the snapshot.

### Brynance

**Finance ingestion, normalization, account tracking, and review.** A Python engine and isolated browser connector, with Electron/React desktop interfaces and SQLite/sql.js persistence.

- **Footprint:** 19,453 implementation LOC in 44 files; no separately classified test/support files in this export.
- **Languages:** Python 12,361 LOC; JSX 4,124; JavaScript 2,567; HTML 401.
- **Form:** Desktop and headless connector source, including an earlier account-review interface. This is engineering evidence, not a claim of a qualified commercial finance product.

### Veylometry

**Product/brand website and presentation experiences.** React/TypeScript and CSS, with Vite/Vinext tooling and PHP/static-hosting artifacts.

- **Footprint:** 4,996 implementation LOC in 52 files; 2 test/support files, 167 LOC.
- **Languages:** TypeScript 2,197 LOC; CSS 2,125; JavaScript 475; PHP, HTML, and SQL.
- **Form:** Website source, review variants, and historical prototypes. The number is not a measurement of only the current live site; optional starter dependencies are not evidence of active production features.

### Aegovra Home

**Earlier home-automation and voice-assistant foundation.** Python/FastAPI/Uvicorn source, an HTTP bridge, and local speech/LLM integration.

- **Footprint:** 657 Python implementation LOC in 14 files; no separately classified test/support files in this export.
- **Form:** Archived foundation and service/CLI source. Current Home application work belongs to Ownce; this is not presented as another current standalone home application.

## Counting method

Counts use [scc 4.1.0](https://github.com/boyter/scc/releases/tag/v4.1.0), with its official release checksum verified, against fourteen clean private source snapshots. Local audit records preserve the exact commits, file hashes, inclusion rules, and exclusions. No implementation source is published with these profiles.

- Counts exclude blank and comment-only lines, documentation, data, dependency trees, generated bundles, and identified generated/reference material. Styles, SQL, native bridges, and operational/build scripts can count as implementation source.
- Ownce's mirrored company sources and proposed changes are excluded. Project Operations' migration tree is excluded conservatively. Native scaffold directories are reviewed separately from custom native code.
- Exact duplicate file bytes are counted once within each repository. Modified variants and near-duplicates remain; cross-project totals are therefore not additive.
- “Test/support” includes path-classified test code, fixtures, and supporting files. It does not count test cases. Inline tests in implementation files cannot be separated by this method.
- Test suites were **not executed for this measurement**. File counts do not imply test coverage, passing results, release readiness, or security certification. A zero means no matching separate files in the reviewed export, not proof that no testing exists elsewhere.
- These snapshots omit runtime/private material and may differ from continuing local development. Source size establishes scope; architecture decisions, working demonstrations, and verified outcomes provide the stronger professional evidence.

For a professional review, discussion can focus on the architecture and decisions behind a selected system, its demonstrated behavior, and the remaining verification work. Source access and deployment access remain private.
