---
trigger: always_on
---

### SYSTEM INSTRUCTION: CONTEXTKEEPER MODE ###

**DESCRIPTION:**
Prevents context loss during long sessions. Acts as a persistent memory anchor, summarizing progress and maintaining goal alignment.

**TRIGGER:**
Activate when the user says "ContextKeeper", "Durum Raporu", "Özetle", "Nerede kaldık?" or after a long sequence of code changes (>5 turns).

**STRICT PROTOCOL:**

1.  **HISTORY SCAN (Geçmiş Taraması):**
    * Review the conversation history.
    * Summarize *what* has been changed and *why*.
    * Recall key decisions (e.g., "We decided to use MVVM to avoid massive View files").

2.  **GOAL ALIGNMENT (Hedef Kontrolü):**
    * State the immediate active goal.
    * Verify if the last few actions align with this goal.

3.  **ACTIVE SCOPE (Dosya Listesi):**
    * List the files currently being modified.
    * Identify related files that might need attention (Dependencies).

4.  **ROADMAP (Yol Haritası):**
    * Define the immediate next step.
    * Show the remaining steps to complete the feature.

**OUTPUT FORMAT (Context Card):**
---
**📍 STATUS REPORT**
* **Current Goal:** [e.g., Refactoring ScanResultView]
* **✅ Completed:**
    * Fixed Danger Card alignment.
    * Updated colors to `.systemGray6`.
* **📂 Active Files:** `ScanResultView.swift`, `HistoryDetailView.swift`
* **🔜 Next Step:** Create reusable `HealthMetricsCard` component.
---