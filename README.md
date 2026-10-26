# 🪄 EventGenie AI — GenAI-Powered Celebration & Event Planner

**EventGenie AI** is an intelligent, single-page application (SPA) built to help users seamlessly plan, organize, and execute **weddings, birthdays, community gatherings, and corporate events**. Powered by Google Gemini AI, it dynamically generates personalized event themes, structured budget breakdowns, phased task timelines, and vendor contact management in a secure, high-performance UI.

---

## 🌟 Key Features

- 🎨 **AI Event Architect:** Generates bespoke event themes, decor concepts, and guest experience ideas using `gemini-2.5-flash` (with a smart client-side fallback engine).
- 💰 **Interactive Budget Planner:** Track estimated vs. actual expenses with live visual progress metrics and category allocations.
- 📋 **Milestone Checklist:** Organized timeline task manager categorized by event phases (e.g., *6-12 Months Out*, *1 Month Out*).
- 📇 **Vendor CRM Directory:** Keep track of caterers, photographers, venues, and entertainment suppliers in one centralized dashboard.
- 🔬 **Built-in Diagnostic Suite ("Self-Check"):** An automated test runner built directly into the UI header to verify security, state mutation, schema parsing, and accessibility live for evaluators.
- 💾 **Data Persistence & Export:** Automatically saves planning data to `localStorage` and provides full JSON export support.

---

## 🛠️ Technical Stack & Architecture

- **Frontend:** HTML5, Tailwind CSS (via CDN), FontAwesome Icons
- **Logic & State:** Vanilla ES6+ JavaScript following a clean **Model-View-Controller (MVC)** design pattern:
  - `StateManager`: LocalStorage sync & immutable state operations
  - `AIService`: Gemini 2.5 API integration + offline Fallback Engine
  - `SecurityUtils`: Strict XSS input sanitization & safe JSON parsing
  - `TestingSuite`: Embedded live unit test and diagnostic runner
  - `UIController`: DOM orchestration & event handling
- **Accessibility:** WCAG AA compliant with keyboard focus traps, ARIA roles, high-contrast colors, and dynamic screen reader announcers (`aria-live`).

---

## 🚀 Getting Started

Since EventGenie AI is built as a lightweight single-file application, no complex Node build steps or server dependencies are required!

1. **Clone or Download the Repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
   cd YOUR_REPO_NAME
