# 📡 SupportLens — Real-Time Video Support Platform

A visually polished, high-performance, single-file frontend template designed for a self-hosted real-time customer video support platform. Built from scratch with semantically clean HTML5, custom-tokenized CSS3 variables, and vanilla JavaScript state handling. 

Developed exclusively as a turnkey presentation interface for the **AtomQuest Hackathon 1.0 Grand Finale**.

---

## 🚀 Vision & Key Selling Points

Modern customer support frequently struggles with "blind communication." SupportLens remedies this by offering immediate, web-based visual context without sacrificing infrastructure autonomy or security.

* **100% Self-Hosted SFU Architecture:** Built conceptually to work seamlessly with an independent server media engine (e.g., Node.js + `mediasoup`), ensuring no third-party media routing APIs touch your streams.
* **Zero-Installation Client Delivery:** Customers access real-time multi-stream infrastructure instantly within native browser boxes without downloading desktop apps, browser extensions, or creating user accounts.
* **Comprehensive Data Sovereignty:** Keeps internal metrics, recording buffers, chat logs, and shared payload storage strictly on local enterprise servers.

---

## 🎨 User Interface Design Architecture

The interface utilizes a custom design token framework built around desaturated, highly professional typography and palettes engineered specifically for enterprise software contexts.

### Color Tokens & Theme
* **🎨 Backgrounds & Canvas:** Soft warm neutrals (`--sand: #F7F3EE`, `--warm-white: #FDFBF8`) eliminate screen glare and reduce eye fatigue for multi-hour support shifts.
* **📂 Typography & Structural Boundaries:** Deep corporate slates (`--slate-800: #2C3440`, `--slate-900: #1A2130`) offer strict readability hierarchies.
* **🌱 Accents & Context Signifiers:** Minimalist corporate teal (`--teal: #1A8A7B`, `--teal-light: #23BCA8`) sets a clean primary brand direction, backed by standard state highlights (Amber for waiting/cam-off, Red for destructive actions/active records, Green for continuous live system states).

### Layout System
Built with strict multi-breakpoint CSS standard rendering rules (`@media (max-width: 1024px)`, `768px`, and `480px`).
* **Desktop Layouts:** Utilize linear grids and side-by-side content tables for continuous monitoring, administrative views, and simultaneous call-room tasks.
* **Mobile-Adapted Layouts:** Automatically compress active dashboards into singular streams, transform large horizontal tracking tables into focus cards, and slide the core sidebar into a hardware-accelerated off-canvas overlay.

---

## ⚙️ Fully Navigable Single-Page Views

The template contains **6 production-ready UI mockups** dynamically controlled via an explicit localized single-page router function (`showPage(id)`):

### 1. Landing Page (`pageLanding`)
An executive overview featuring a stylized navigation header, immediate access routing for agents and customers, core service value propositions, an asset-free simulated 16:9 browser call frame, and an architecture footer block.

### 2. Authentication Gateway (`pageAuth`)
A centralized credential interface supporting seamless toggle interactions between existing Agent Sign-In routes and new corporate registration workflows. Includes role select cards complete with visual indicator changes.

### 3. Comprehensive Agent Dashboard (`pageDashboard`)
The central mission-control zone for helpdesk operators, modularly split across four functional tracking panels:
* **Overview Panel:** High-visibility metric highlights track session counts, online customer queues, daily traffic thresholds, and average call resolutions, followed by a dynamic interactive Active Sessions workspace table.
* **Sessions Panel:** A detailed view for managing existing sessions, generating customer access code pairs, or closing active sessions.
* **Recordings Panel:** Provides deep-dive management features for historical video content, displaying file sizes, validation states, and discrete operational download assets.
* **History Panel:** A searchable, persistent ledger log recording start parameters, end parameters, and structural event summaries for past interactions.

### 4. Live Call Room (`pageCall`)
An expansive full-viewport call console designed to capture immediate visual status data:
* **Media Grid Matrix:** Dynamic 16:9 viewports displaying localized stream feedback blocks, custom speaking state frames, camera-state overlays, and HD network badges.
* **Hardware Control Dock:** Centered tactical controls for Mic Mute state, Camera Toggle state, localized Screen Share simulations, and Call Termination. Includes an agent-only recording trigger option.
* **Context Control Center:** A tabbed sidebar layout containing a complete chat console with inline attachment upload styling, real-time message metadata, and an explicit active participant register.

### 5. Client Joining Portal (`pageJoin`)
A clean, secure portal for incoming users that parses automated token lines, provides immediate host identification summaries, and securely queries explicit device microphone and camera capture authorization.

### 6. System Administration Panel (`pageAdmin`)
An analytical framework for operational monitoring teams. Provides active cross-agent monitor routes, system health bars tracking CPU/Memory/Bandwidth allocations, real-time SFU network performance feedback, and live event log summaries.

---

## 🛠 Structural Mechanics & State Engine

The frontend layout relies entirely on atomic vanilla components, completely eliminating heavy runtime framework dependencies:

* **View-Switching Logic:** Page states and tabular workspaces utilize standard class manipulations (`.classList.toggle('hidden')`, `.classList.add('active')`) to guarantee immediate rendering responses without frame drops.
* **Dynamic Data Compiling:** Session creation methods ingest structural input parameters on the fly, programmatically injecting fresh, interactive component strings into active document blocks using `insertAdjacentHTML`.
* **Media Interconnectivity Simulation:** Active state logic models accurate stream actions, handling microphone parameters, toggling camera viewports, tracking recording timelines, and updating badge statuses across matching indicators.
* **Communication Persistence:** The embedded chat system features independent layout managers that sanitize raw string payloads using `escapeHtml`, automatically generate time tokens, handle vertical anchor tracking via `scrollTop`, and adapt alignment fields to separate user contexts.
* **Operational Alerts System:** A self-purging multi-state toast engine dynamically appends customized message components into independent floating target wrappers (`#toastContainer`), handling asynchronous animations and clean node removal steps after predefined execution frames.
* **Accessibility Keybindings:** Includes physical keyboard shortcuts to streamline interaction workflows for active power users during high-pressure support situations (`M` for localized audio toggles, `V` for instant camera state shifts).

---

## 📂 Quick Start Deployment

Because the platform is engineered completely inside a unified single-file HTML wrapper, execution requires zero compilation overhead:

1. Clone or download the source repository files to your local system environment.
2. Open the file `video-support-platform.html` directly in any contemporary evergreen browser engine (Chrome, Safari, Firefox, Edge).
3. **To evaluate the full platform workflow:**
    * Click **Agent Login** on the landing navigation bar.
    * Click the **Sign in** button on the Auth screen to bypass using the preloaded demo credentials (`agent@supportlens.app` / `demo1234`).
    * Interact with dashboard states, generate new session assets, copy invite tokens, or launch directly into the **Join** view to experience the full operational environment.
