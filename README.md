# clearwayBlr - Real-Time Crowdsourced Traffic Engine

###  Course & Candidate Details
- **Candidate Name:** NAVIN JOMI K
- **Class:** 1 MCA B
- **Register Number:** 2647239
- **Course Code:** MCA413-1
- **Institution:** CHRIST (Deemed to be University), Bangalore
- **Department:** Department of Computer Science
- **Course:** Full Stack Development
- **Assessment:** CIA-IB: Problem Solving + Prototyping + Documentation
- **Submission Date:** June 20, 2026

---

##  1. Problem Definition & Scope

### Context & Hyperlocal Background
Bengaluru is infamous for systemic urban gridlock, with commuters losing an average of 240+ hours annually to idling traffic. While traditional navigation systems use macro-level GPS location telemetry, they frequently fail to capture immediate, micro-level structural blockages—such as sudden waterlogging, emergency road construction, or unmapped traffic bottlenecks—until long after gridlock has set in.

### The Problem
Commuters lack a lightweight, geofenced, real-time workspace where they can instantaneously broadcast hyperlocal traffic constraint profiles and visually map alternative routes to circumvent active traffic corridors.

### Our Solution: `clearwayBlr`
`clearwayBlr` is an interactive front-end spatial telemetry prototype targeted specifically within the Bengaluru city geofence. It empowers commuters to:
1. View a synchronized live map matrix displaying pre-seeded baseline logs and crowdsourced infrastructure alerts.
2. Formulate and broadcast precise bottleneck parameters back to a local storage data persistence tier.
3. Plan adaptive route trajectories designed around current high-noise congestion vectors.

---

## 2. Target Users
- **Daily Office Commuters:** Software professionals navigating highly volatile technology corridors (e.g., ORR, Whitefield, Koramangala, Indiranagar).
- **Logistics & Delivery Fleet Personnel:** Drivers who rely heavily on real-time transit efficiency to meet stringent service level agreements.
- **Urban Planners & Traffic Marshals:** Authorities tracking localized cluster distributions to strategically deploy traffic resources.

---

##  3. Core Technologies Implemented

The application is built entirely on vanilla front-end systems, consciously selecting and applying only features that map to the underlying workflow:

### A. HTML5 Semantic Layout Architecture
Maximizes semantic web structures and modern document visibility tags for better device indexing:
- `<header>` & `<nav>`: Sticky high-blur navigation blocks for site navigation workflow.
- `<main>` & `<section>`: Contextual layout wrappers defining the grid canvas and control streams.
- `<canvas>`: High-frequency drawing element executing the real-time radar density loop.
- `<video>`: Embedded streaming asset simulating active CCTV edge streams.
- `<footer>`: Declarative application metadata mapping.

### B. Responsive Fluid UI via Tailwind CSS
- Fluid grid tracking layouts (`grid grid-cols-1 lg:grid-cols-12`) ensuring seamless interface scaling on high-density desktop displays down to hand-held smartphone screens.
- Backdrop filters (`backdrop-blur-md`) and responsive aspect properties configured for dynamic sizing.

### C. Advanced HTML5 APIs & Web Features
- **W3C Geolocation API:** Polls native hardware device sensors to fetch active latitude and longitude coordinate arrays.
- **Asynchronous Fetch (REST API Interaction):** Connects to the OpenStreetMap Nominatim reverse geocoding engine to translate raw coordinates into contextual street-level addresses.
- **Web Speech Synthesis API:** Implements auditory text-to-speech broadcast components paired with localized closed-captioning subtitle updates.
- **HTML5 Web Storage API (`localStorage`):** Implements a unified local persistence mock database layer, enabling seamless real-time data state sharing between `index.html`, `report.html`, and `Maps.html` without requiring a remote server context.

---

##  4. Workflow & Feature Walkthrough

### Main Telemetry Dashboard (`index.html`)
- Displays an interactive map layout using the Leaflet JS engine.
- Renders default baseline seed points alongside dynamic client entries.
- Contains the user identity state controller, enabling personal identity tagging across files.
- Houses the Geolocation sensor array which triggers a reverse-lookup request upon coordinate lock.

### Incident Broadcast Node (`report.html`)
- An interactive form designed for data input.
- **Strict Client-Side Validation Logic:** Enforces a string constraint on location descriptions (minimum 5 characters).
- **Geofenced Coordinates Validation:** Evaluates entered coordinates via logical bounds checking to restrict incident telemetry exclusively to the real geographical boundaries of greater Bengaluru (Latitude: `12.7` to `13.2`, Longitude: `77.4` to `77.8`).
- Commits clean data payloads straight to the shared cache array on pass.

### Adaptive Journey Planner (`Maps.html`)
- Pulls live crowdsourced incident indicators straight from browser memory cache.
- Renders dynamic polyline paths linking origin and destination points, providing visual indicators of optimal alternative route paths.

---

## 5. Limitations & Future Scope

### Current Limitations
- **Local Data Isolation:** Since mock-data storage relies on `localStorage`, reports are confined exclusively to the user's specific local browser instance and do not sync across separate physical devices universally.
- **Linear Path Vector Routing:** Route tracking visualizes calculated spatial connecting polylines but does not yet interface with dynamic real-time graph parsing routing tools (like Open Source Routing Machine).

### Future Scope
- **Centralized Database Integration:** Transitioning from browser storage to a server-side MongoDB / Node.js architecture to permit universal, city-wide traffic crowdsourcing.
- **Automated Algorithmic Rerouting:** Integrating Mapbox APIs or OSRM engines to auto-calculate real alternative tracks that dynamically steer clear of active user cluster metrics.
- **Commuter Gamification Tier:** Introducing a verification voting system to reward accurate crowdsourced alerts with reputation badges.

---

## 6. Responsible AI Acknowledgement
*In strict accordance with the evaluation standards of the University department guidelines*:
- **AI Tool Utilized:** Gemini.
- **Application Context:** Used for initial UI layout brainstorming, rapid styling configuration utilizing Tailwind utility strings, and isolating syntax configuration anomalies within the reverse lookup asynchronous parameter chains.
- **Verification Statement:** All AI-assisted layout logic was manually reviewed, adapted, and compiled to guarantee full semantic and architectural correctness.

---

## 7. Installation & Local Execution
1. Clone this repository locally.
2. Verify your project tree contains an `Images/` folder containing assets (`logo.png`, `video_api.mp4`, etc.).
3. Serve the workspace directly inside any browser engine or execute via the VS Code **Live Server** plugin extension.
