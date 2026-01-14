---
trigger: always_on
---

### SYSTEM INSTRUCTION: STEP-BY-STEP MODE ###

**DESCRIPTION:**
A strict protocol for executing complex tasks sequentially. Prevents overwhelming changes by enforcing atomic operations and verification.

**TRIGGER:**
Activate when the user says "Step by step", "Adım adım", "Tane tane", "Tek tek ilerle" or "Don't rush".

**STRICT PROTOCOL:**

1.  **ATOMIC PLANNING (Atomik Planlama):**
    * Before writing any code, list all necessary steps.
    * Each step must be **atomic** (changing one function, one file, or one logic block).
    * *Rule:* Do not group unrelated changes into a single step.

2.  **SINGLE FILE FOCUS (Tek Dosya Odağı):**
    * NEVER modify multiple files simultaneously unless they are tightly coupled interfaces.
    * Focus on the current file, finish it, verify it, then move to the next.

3.  **VERIFICATION LOOP (Doğrulama Döngüsü):**
    * **After each step:** Ask the user "Does this look correct?" or "Did the build pass?".
    * **Automated Check:** If possible, suggest running a specific test case for that step.

4.  **HALT ON FAILURE (Hata Duruşu):**
    * If a step fails or introduces a bug, **STOP IMMEDIATELY**.
    * Do not proceed to Step 2 if Step 1 is broken. Fix Step 1 first.

**OUTPUT FORMAT:**
Display the progress at the start of your response:
* [✅] Step 1: Database Schema Update (Completed)
* [🔄] **Step 2: Update User Model (Current Task)**
* [ ] Step 3: Migration Script (Pending)