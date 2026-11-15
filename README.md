# Awesome-Office-Document-Collaboration-CO-Authoring

# Awesome Office Document Collaboration & Co-authoring

> A curated list of top Office Document Collaboration and Co-authoring platforms — both SaaS/Hosted commercial solutions and open-source alternatives for real-time co-editing, comments, and version control across Word, Excel, and PowerPoint formats.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Microsoft 365](#microsoft-365)
  - [Google Workspace](#google-workspace)
  - [Zoho Docs](#zoho-docs)
  - [Quip](#quip)
  - [Box Notes](#box-notes)
  - [Dropbox Paper](#dropbox-paper)
- [Open-Source Software](#-open-source-software)
  - [ONLYOFFICE Docs](#onlyoffice-docs)
  - [Nextcloud Write](#nextcloud-write)
  - [Collabora Online](#collabora-online)
  - [Diwan](#diwan)
  - [CryptPad](#cryptpad)
  - [Etherpad](#etherpad)
  - [HedgeDoc](#hedgedoc)
  - [TypstPad](#typstpad)
  - [La Suite Docs](#la-suite-docs)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Office Document Collaboration and Co-authoring platforms. These are not open-source but are included as reference points for feature comparison.

### Microsoft 365
**Type:** Office apps with real-time co-authoring
Microsoft 365 provides Word, Excel, and PowerPoint Online with real-time co-authoring, comments, and track changes. It is the default choice for organizations standardized on Microsoft, with seamless transition to desktop apps for advanced formatting.

### Google Workspace
**Type:** Real-time collaborative documents
Google Workspace (Docs, Sheets, Slides) provides live cursors, comments, and suggestion mode, with deep integration into Google Drive. It is the most widely adopted cloud document suite, with zero setup and strong cross-platform support.

### Zoho Docs
**Type:** Document collaboration within Zoho ecosystem
Zoho Docs provides document editing and collaboration as part of the broader Zoho suite, with integration into Zoho CRM and Projects. It is the natural choice for organizations already using Zoho products.

### Quip
**Type:** Collaborative documents within Salesforce ecosystem
Quip (Salesforce) provides collaborative documents and spreadsheets with integrated chat and comments. It is the natural choice for Salesforce customers wanting document collaboration tied to CRM records.

### Box Notes
**Type:** Collaborative notes within Box content platform
Box Notes provides real-time collaborative document editing integrated with Box storage. Suited for teams already using Box for content management wanting lightweight document collaboration.

### Dropbox Paper
**Type:** Collaborative docs integrated with Dropbox
Dropbox Paper provides collaborative document editing with a clean, minimalist interface, integrated with Dropbox storage. Suited for teams already using Dropbox for file storage wanting lightweight document collaboration.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Office Document Collaboration and Co-authoring tools. The open-source ecosystem spans **full Office-compatible suites**, **sovereign Nextcloud integrations**, **single-binary office suites**, and **specialized Markdown/Typst editors**.

### ONLYOFFICE Docs
**Stack:** JavaScript / Node.js / Docker | **License:** AGPL-3.0 (Community)
ONLYOFFICE Docs is the most widely adopted open-source Office-compatible suite, rated #1 in a 2026 comparison of collaborative document software [citation:5]. Key capabilities include:
- **Real-time co-editing** with paragraph-level locking, so two or more users can edit the same document simultaneously [citation:10]
- **High Office format fidelity** — DOCX, XLSX, PPTX open and save without losing layout [citation:10]
- **Plugin system** for macros, translation tools, and templates
- **Self-hosted document server** for privacy
- **Free community edition** for up to 20 simultaneous connections, with enterprise licenses for larger deployments [citation:10]

It integrates with many file sync platforms and is the go-to choice when Office compatibility is non-negotiable.
**Best for:** Teams needing near-perfect Microsoft Office format fidelity in a self-hosted collaborative editor, accepting the 20-connection limit on the free tier.

### Nextcloud Write
**Stack:** PHP / Nextcloud Office (Collabora or Euro-Office) | **License:** AGPL-3.0
Nextcloud Write is a full-featured, real-time collaborative document editor that runs entirely on infrastructure of your choice, positioned as a sovereign open-source alternative to Word and Google Docs [citation:4]. Key features include:
- **Real-time co-editing** with colored cursors and a formal review mode for tracking edits and accepting/rejecting changes
- **Granular sharing** via internal permissions or public links (read-only, editable, or watermarked)
- **Federated collaboration** allowing teams on separate Nextcloud instances to co-author across servers [citation:4]
- **Automatic saving and version history**, with compare-and-combine tools for reconciling divergent versions
- **DOCX and ODT support**, ensuring documents remain intact across software
- **Offline editing** with sync on reconnection
- **AI assistant** via Nextcloud Assistant, with administrator control over local vs. trusted provider models [citation:4]

Deploys as part of Nextcloud Office, which also includes spreadsheet and presentation editors. You can run it with either Euro-Office (client-centric, Office-compatible) or Collabora Online (server-centric, OpenDocument-focused) [citation:4].
**Best for:** Organizations already running Nextcloud or prioritizing data sovereignty wanting a complete document suite with federation and full data control.

### Collabora Online
**Stack:** C++ / LibreOffice core / Docker | **License:** MPL-2.0 (Community)
Collabora Online is an open-source collaborative office suite built on the LibreOffice engine, with a server-centric architecture where the server does the heavy lifting [citation:4]. It prioritizes the OpenDocument Format (ODT/ODS/ODP) while supporting Office formats, and integrates with Nextcloud, ownCloud, and other file sync platforms. It is rated among the top collaborative document tools in 2026 comparisons [citation:5]. **Trade-off:** Office format fidelity is not as precise as ONLYOFFICE, and the server-centric model requires more server resources.
**Best for:** Organizations prioritizing OpenDocument standards and deep LibreOffice compatibility, particularly those already using Collabora within Nextcloud.

### Diwan
**Stack:** Go / CRDT (Yjs) | **License:** MIT
Diwan is a self-hostable, real-time collaborative office suite delivered as a **single Go binary with the entire frontend embedded** — one file to deploy [citation:9]. Key features include:
- **Documents** with rich-text editing (TipTap), anchored comments, suggestions with accept/reject, version history with restore, find/replace, and live outline [citation:9]
- **Spreadsheets, Slides, Whiteboards, and PDF signing** as part of the same suite
- **CRDT-based peer-to-peer collaboration** — Docs and whiteboards sync as Yjs updates, with end-to-end-encrypted rooms where the key never reaches any server [citation:9]
- **No account, no cloud, no external service required** — runs standalone with local storage by default
- **Every editor published as an npm library** (`diwan` package), so you can embed any surface in your own app [citation:9]

**Trade-off:** Documents are one surface of a broader suite rather than a standalone Word replacement, and the project is newer than ONLYOFFICE or Nextcloud.
**Best for:** Privacy-focused teams wanting a self-contained, single-binary office suite with peer-to-peer encrypted collaboration, accepting a newer ecosystem.

### CryptPad
**Stack:** JavaScript | **License:** Open Source
CryptPad is a privacy-first, open-source collaboration suite offering **end-to-end encrypted** alternatives to Google Docs, with over **200,000 monthly users** and **1,500+ self-hosted instances** . Users can co-edit documents, manage Kanban boards, host whiteboard sessions, and create forms — all without exposing content to the server or admins. Unlike traditional tools, only collaborators can access the data they create and share, with zero-knowledge architecture . It is recommended by Privacy Guides for its strong encryption and transparent development.
**Trade-off:** Format compatibility and feature depth trail ONLYOFFICE; it prioritizes encryption over Office fidelity.
**Best for:** Teams with strict confidentiality requirements (legal, activist, privacy-sensitive) needing real-time collaboration without trusting the server operator with content.

### Etherpad
**Stack:** Node.js | **License:** Apache-2.0
Etherpad is a long-standing open-source real-time collaborative editor, rated among the top collaborative document tools in 2026 comparisons [citation:5][citation:14]. It provides simple, reliable real-time text co-editing with colored cursors and basic formatting. **Trade-off:** It is a plain-text/rich-text editor rather than an Office format suite — no DOCX compatibility or spreadsheet features.
**Best for:** Teams needing lightweight, reliable real-time text collaboration without Office format requirements.

### HedgeDoc
**Stack:** Node.js / React | **License:** AGPL-3.0
HedgeDoc (formerly CodiMD) is an open-source Markdown editor for self-hosted use with real-time shared editing [citation:5][citation:14]. It is positioned for technical teams wanting collaborative Markdown documents with live preview, rather than Word/Excel format compatibility.
**Best for:** Technical teams wanting real-time collaborative Markdown editing, accepting that it is not an Office document replacement.

### TypstPad
**Stack:** Go / Typst / Yjs | **License:** Open Source
TypstPad is a self-hosted collaborative **Typst document editor**, positioned as "Overleaf for Typst" [citation:3]. Key features include:
- **Real-time collaboration** with live cursors and presence (Yjs CRDT, merges never conflict)
- **Live preview** with Typst compiled to WASM, with fonts and packages served by your own server
- **SSO** via generic OIDC (Keycloak, Authentik, Google, Azure AD) plus built-in email/password
- **Version history** with automatic snapshots, named versions, visual diffs, and one-click restore
- **Suggestions mode** with tracked changes and threaded comments
- **AI integration** via REST API, MCP server, and CLI for agents like Claude [citation:3]

**Trade-off:** Typst is a typesetting system, not an Office format — it does not edit DOCX or XLSX.
**Best for:** Technical and scientific teams writing structured documents with Typst, wanting collaborative editing with modern AI integration.

### La Suite Docs
**Stack:** Django / Next.js / ProseMirror / Yjs | **License:** MIT
La Suite Docs is an open-source collaborative editor positioned as a sovereign alternative to Notion or Google Docs, backed by the German Center for Digital Sovereignty (ZenDiS) and the French DINUM. It provides rich-text and Markdown editing with slash commands, real-time collaboration with live cursors and comments, subpages and hierarchy, and import/export to DOCX and Markdown. **Trade-off:** It is a block-based document editor rather than an Office format suite — no spreadsheet or presentation capabilities.
**Best for:** Public institutions and teams wanting a sovereign, Notion-style document editor with strong European government backing.

---

## 📊 Comparison at a Glance

| Software | License | Stack | DOCX/Office | Real-Time Co-Edit | Self-Hosted | Best For |
|----------|---------|-------|-------------|-------------------|-------------|----------|
| **Microsoft 365** | Proprietary | Cloud | ✅ Native | ✅ | ❌ | Microsoft ecosystem |
| **Google Workspace** | Proprietary | Cloud | ✅ | ✅ | ❌ | Universal collaboration |
| **ONLYOFFICE Docs** | AGPL-3.0 | JS/Docker | ✅ High fidelity | ✅ | ✅ | Office-compatible co-editing |
| **Nextcloud Write** | AGPL-3.0 | PHP/Nextcloud | ✅ | ✅ | ✅ | Sovereign full suite + federation |
| **Collabora Online** | MPL-2.0 | C++/LibreOffice | ✅ (ODF-first) | ✅ | ✅ | OpenDocument standards |
| **Diwan** | MIT | Go/CRDT | (Check) | ✅ P2P | ✅ | Single-binary encrypted suite |
| **CryptPad** | Open Source | JavaScript | (Limited) | ✅ E2EE | ✅ | Maximum privacy |
| **TypstPad** | Open Source | Go/Typst | ❌ (Typst) | ✅ | ✅ | Typst scientific docs |
| **Etherpad** | Apache-2.0 | Node.js | ❌ | ✅ | ✅ | Lightweight text co-editing |
| **HedgeDoc** | AGPL-3.0 | Node.js | ❌ (Markdown) | ✅ | ✅ | Markdown collaboration |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Office Document Collaboration or Co-authoring tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The Office document co-authoring space splits between **full Office-format suites** (ONLYOFFICE Docs for the highest Office fidelity with paragraph-level locking, Nextcloud Write for sovereign integration with federation and AI, Collabora Online for OpenDocument standards) and **specialized editors** (CryptPad for end-to-end encryption, TypstPad for Typst typesetting, HedgeDoc for Markdown, Etherpad for plain-text co-editing). **ONLYOFFICE Docs** is the clear choice when DOCX/XLSX/PPTX compatibility is the priority, rated #1 in a 2026 comparison [citation:5][citation:10]. **Nextcloud Write** is the strongest option for organizations wanting a complete sovereign office suite integrated with their existing Nextcloud deployment, with federated collaboration across instances [citation:4]. For privacy-critical contexts, **CryptPad** offers genuine end-to-end encryption that no other tool on this list matches . **Diwan** is a notable newer entrant delivering a full office suite as a single Go binary with peer-to-peer encrypted rooms [citation:9].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
