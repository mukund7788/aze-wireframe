# AZE AI — Prototype & Wireframe Hub

[![Live Demo](https://img.shields.io/badge/Live_Hub-GitHub_Pages-0D6EFD?style=for-the-badge&logo=github)](https://mukund7788.github.io/aze-wireframe/)
[![Design System](https://img.shields.io/badge/Design_System-Zignuts_AZE-061D42?style=for-the-badge)](https://zignuts.com)
[![Prototypes](https://img.shields.io/badge/Prototypes-6_Modules-10B981?style=for-the-badge)]()

Central catalog and live interactive prototype hub for the **AZE AI Voice Assessment & Automated CEFR Scoring Platform**.

🌐 **Live URL:** [https://mukund7788.github.io/aze-wireframe/](https://mukund7788.github.io/aze-wireframe/)

---

## 🚀 Overview

The **AZE Wireframe Hub** brings all interactive UX prototypes, feature simulators, and product specifications into a unified master application shell. It allows cross-functional teams (Product Managers, Technical BAs, Frontend/Backend Engineers, and Enterprise Stakeholders) to inspect, interact with, and validate system behaviors before code implementation.

### Key Capabilities
* **Central Navigation Hub:** Switch seamlessly between all 6 platform wireframes via hash routing (`#self_service_demo`, `#cost_dashboard`, etc.).
* **Responsive Viewport Simulator:** Test layouts instantly across **Desktop (100%)**, **Tablet / Laptop (1024px)**, and **Mobile Device Frame (414px)**.
* **Instant Standalone Access:** Open any wireframe directly in a standalone browser tab with one click (`↗ Open Standalone`).
* **Real-Time Search:** Filter through prototypes and feature specifications directly in the sidebar.

---

## 📦 Wireframe Catalog

| Category | Module Hash | Wireframe File | Description |
| :--- | :--- | :--- | :--- |
| **Overview** | `#wireframe_info` | Built-in Hub Guide | Platform background, wireframing methodology, and architecture guide. |
| **Client Portal** | `#self_service_demo` | [`self_service_demo_client_portal_wireframe.html`](self_service_demo_client_portal_wireframe.html) | Corporate email signup validation, pristine zero-state client account (15 students / 15 tests quota), Claude-style full-screen showcase overlay modal, Available Tests sidebar widget, and Buy Tests subscriptions. |
| **Client Portal** | `#group_results` | [`group_results_client_portal_wireframe.html`](group_results_client_portal_wireframe.html) | Multi-candidate group performance reporting, CEFR score distributions across Speaking, Listening, Reading, and Writing, exportable summaries, and cohort filtering. |
| **Cost Governance** | `#cost_dashboard` | [`third_party_cost_dashboard_wireframe.html`](third_party_cost_dashboard_wireframe.html) | Third-party AI cost and anomaly monitoring dashboard for OpenAI, AWS Bedrock, and SpeechAce USD billing with spike detection and student attribution. |
| **Cost Governance** | `#cost_estimator` | [`cost_estimator_wireframe.html`](cost_estimator_wireframe.html) | Budget simulation tool calculating token consumption, audio processing duration, model pricing tiers, and projected per-assessment costs. |
| **Assessment Studio** | `#question_clusters` | [`question_fields_cluster_wireframe.html`](question_fields_cluster_wireframe.html) | Assessment question authoring interface for multi-prompt voice items, rubric scoring weights, and recording constraints. |
| **Specifications** | `#interactive_brd` | [`AZE_BRD_Interactive_v4.html`](AZE_BRD_Interactive_v4.html) | Interactive Business Requirements Document (BRD) and technical specification viewer. |

---

## 🛠️ Local Development & Preview

To run the hub locally on your machine:

```bash
# Clone the repository
git clone https://github.com/mukund7788/aze-wireframe.git
cd aze-wireframe

# Start a local static HTTP server (Python 3)
python3 -m http.server 8080

# Open in your browser
# http://localhost:8080
```

---

## 🎨 Design System & Theming Tokens

Built adhering strictly to the **Zignuts & AZE Enterprise Design System**:
* **Typography:** `Poppins` (Bold 700 / SemiBold 600 / Medium 500) for headers, `Inter` / `Nunito` for UI elements, `JetBrains Mono` for telemetry and contracts.
* **Color Tokens:**
  * **Zignuts Royal Blue:** `#0D6EFD`
  * **Deep Navy:** `#061D42`
  * **Signature Gradient:** `linear-gradient(135deg, #FE765A 0%, #8E75D2 50%, #2B98F9 100%)`
  * **Ice Blue:** `#DBEEFF`
  * **Neutral Slate:** `#64748B`, `#E2E8F0`, `#F8FAFC`

---

## ➕ Adding a New Wireframe

To add a new prototype to the hub:
1. Place your standalone HTML file in the root directory (e.g., `new_feature_wireframe.html`).
2. Open `index.html` and add an entry to the `MODULES` object:
   ```javascript
   'new_feature': {
     title: 'Feature Name',
     category: 'Category Name',
     desc: 'Short summary of the prototype.',
     file: 'new_feature_wireframe.html'
   }
   ```
3. Add a corresponding `<li>` link inside the appropriate `.nav-group` in `index.html`.
4. Commit and push to `main` — GitHub Pages updates automatically!

---

**Maintained by:** Mukund Patil ([@mukund7788](https://github.com/mukund7788))  
**Organization:** Zignuts Technolab / AZE Voice AI
