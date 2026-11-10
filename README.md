# ⏱️ Workflow Timer

A lightweight, single-file productivity and deliverable tracking web application designed for output-based professionals. **Workflow Timer** combines flexible countdown and stopwatch tracking, live deadline projections, visual productivity analytics, a folder-based rich-text notepad, and custom resource bookmarking—all stored locally in your browser with zero backend dependencies.

---

## ✨ Key Features

### 1. Flexible Deliverable Timer
* **Three Tracking Modes:** Choose between **Timer (Countdown)**, **Stopwatch (Elapsed)**, or **Both** simultaneously depending on whether your task has a fixed target duration or open-ended tracking.
* **Live Time Targets Summary:** Automatically calculates and displays your projected completion clock time (e.g., *"File 1 must be completed on 02:30:00 PM"*) and locks in the deadline the moment you start.
* **Custom Audio Notifications:** Built-in Web Audio API double-beep (`beep-beep`) alerts notify you when **5, 10, 15, or 30 minutes** remain on your target timer, complete with a **Test Beep** button and quick toggle switch.
* **Workspace Modes:**
  * **Dark Mode:** High-contrast dark theme toggle persisted across sessions.
  * **Compact Mode:** Scales down spacing and typography for split-screen multitasking.
  * **Focus Mode:** Hides navigation headers and secondary tabs to display only **File Details** and **Workflow Timer**.

### 2. Unified Productivity Dashboard & Output Log
* **KPI Summary Cards:** Real-time calculation of **Total Files**, **Total Active Hours**, **On-Time Rate**, and **Daily Average**.
* **Collapsible 3-Month Activity Heatmap:** Visualizes daily output volume across the current and previous two months with interactive hover tooltips.
* **Collapsible Performance Trend Chart:** Powered by **Chart.js**, comparing *Time Taken* against *Target Time* (in minutes) for recent deliverables.
* **Integrated Files & Output Performance Table:**
  * **Full Filtering & Search:** Filter logs by **Year**, **Month**, **Status** (*On Time*, *Overtime*, *Stopwatch Only*), **Start/End Date Range**, or **File Name** search.
  * **Manual Logging & Editing:** Add past deliverables manually or edit existing entries inline.
  * **Reporting & Exports:** Generate print-ready **PDF Summary** reports, export filtered logs to **CSV**, or create full **JSON** backups.

### 3. Folder-Based Rich-Text Notepad
* Powered by **Quill.js** with formatting tools (headers, font sizes, bold/italic/underline, colors, alignment, lists, links, and pasted images).
* Organize notes into custom **Folders** with reordering, renaming, and 50-step Undo/Redo history.

### 4. Custom Resources Launcher
* Pin frequently used tools, dashboards, and documents as color-coded link pills with selectable **Lucide** icons and custom color swatches.

### 5. Local-First Data Backup & Restore
* All logs, notebook folders, custom resource links, and UI preferences are saved automatically in browser `localStorage`.
* Use **Export Backup** and **Import Backup** (`.json`) to transfer or safeguard your workspace across browsers.

---

## 🛠️ Tech Stack

* **Core:** HTML5, CSS3, Vanilla JavaScript (ES6+)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (CDN) & custom CSS variables/themes
* **Icons:** [Lucide Icons](https://lucide.dev/)
* **Charts:** [Chart.js](https://www.chartjs.org/)
* **Rich-Text Editor:** [Quill.js v2](https://quilljs.com/)
* **CSV Parsing/Export:** [PapaParse](https://www.papaparse.com/)
* **Celebration Effects:** [Canvas Confetti](https://github.com/catdad/canvas-confetti)

---

## 🚀 Getting Started

Because **Workflow Timer** is built as a self-contained single-page HTML application, no build step or server installation is required:

1. Download or clone the repository containing `workflow-timer.html` (or `index.html`).
2. Open the HTML file directly in any modern web browser (Chrome, Edge, Firefox, Safari).
3. Enter your **File Name**, select your **Mode** (*Timer*, *Stopwatch*, or *Both*), set your **Target Time (`HH:MM:SS`)**, and click **Start**.

---

## ⚠️ Disclaimer

This tool is built for personal productivity and time-tracking use. All data is stored locally in your browser's `localStorage`—remember to export a JSON backup periodically before clearing browser site data or switching devices.
