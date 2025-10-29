## 🧠 Artifact 1 — Minimal PRD Prompt (C-L-A-R Format)

**Prompt:**

> **C (Context):** You are an AI product manager helping to draft a minimal Product Requirements Document (PRD) for a lightweight Streamlit application called _Prompt Genius_. The app lets users write, version, and store AI prompts with notes and tags.
> 
> **L (Limits):** Keep it short and incomplete on purpose. Focus only on the most essential sections needed to start development. Avoid implementation details or design mockups.
> 
> **A (Action):** Write a concise PRD scaffold with clear sections for Purpose, Users, Core Features, Non-Goals, and Open Questions. Leave several fields intentionally blank to encourage iteration.
> 
> **R (Result):** Output the PRD in Markdown format.

---

## 📄 Artifact 2 — Sample Minimal PRD Output

```markdown
# Prompt Genius — Minimal PRD (v0.1)

## Purpose
Provide developers and researchers a simple interface to write, store, and iterate on AI prompts.

## Target Users
- Developers exploring AI workflows
- Analysts managing reusable prompts
- Students learning structured prompting

## Core Features
- Create, edit, and tag prompts  
- Save prompt versions with short notes  
- Export or copy prompt text easily  
- (Placeholder for future ideas…)

## Non-Goals
- No authentication or database persistence in MVP  
- No collaborative editing (single-user only)

## Open Questions
- How should versioning be tracked?  
- What metadata should be stored with each prompt?  
- Should AI output examples be saved?  

---

### Artifacts to Create Later
- **ADR 001:** Decision on storage approach (local vs. cloud)
- **README:** Describe purpose, quickstart, and dependencies
- **TODOs:** Track incomplete ideas or future improvements
- **QA Assertions:** Define simple “it works when…” checks
```

---

## 🧪 Artifact 3 — Lab Exercise Handout

**Objective:**  
Use the provided PRD prompt to bootstrap your own _Prompt Genius_ concept.

Excellent — yes, let’s run a professional “QA pass” on your **Prompt Genius Lab** to make sure it meets your intent:
✅ **high impact**,
✅ **minimal time investment**, and
✅ **minimal cognitive load (“minimal Cohn”)** for your developer audience.

---

## 🔍 Review Summary

### 🎯 Overall Alignment

**Intent:** Teach developers that prompt engineering ≈ product design by having them *create a PRD* and a few supporting artifacts.
**Approach:** Guided scaffolding, not completion.
**Verdict:** ✅ Spot on — it hits the right cognitive level.

---

## ✅ Strengths

1. **Low entry barrier**

   * Starts with a simple copy-paste PRD prompt (no setup required).
   * Immediate payoff: they see a working PRD output in <3 minutes.
   * Streamlit mention is *optional*, not blocking.

2. **Clear scaffolding**

   * Each artifact (PRD → ADR → README → To-Dos → QA assertions) naturally builds on the previous one.
   * They can stop at any stage and still feel successful.

3. **Right level of incompleteness**

   * Encourages iteration without overwhelming them.
   * Developers will intuitively fill gaps in the PRD.
   * Perfect for demonstrating “LLM as collaborator” rather than “LLM as oracle.”

4. **Time-boxed flexibility**

   * Can be completed in ~45 minutes or stretched to a few hours.
   * Every phase is standalone (no long dependency chain).

5. **Cognitive flow**

   * Moves from *generation* → *iteration* → *reflection* → *expansion*.
   * Matches how developers learn best (build → debug → reason).

---

## ⚙️ Light Refinements (to make it bulletproof)

| Area                    | Issue                                                               | Fix                                                                                                        |
| ----------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Step 1 Instructions** | Doesn’t explicitly tell them to *save the PRD*                      | Add a line: “Save your generated PRD as `docs/PRD.md`.”                                                    |
| **Step 2 ADR example**  | “Documenting our first architectural choice” is slightly open-ended | Add a small hint: “e.g., Local storage vs. hosted database.”                                               |
| **Step 3 Prototype**    | The Streamlit portion may intimidate complete beginners             | Add one reassuring line: “If Streamlit feels too heavy, just outline your UI as Markdown — that’s enough.” |
| **Step 4 Reflect**      | Excellent, but you could reinforce the self-teaching goal           | Add: “Ask the model: *How could I improve this prompt next time?*”                                         |
| **Advanced Steps**      | All good — very strong, but could use a “stop point” suggestion     | Add: “You can stop after Step 2 and still complete the lab successfully.”                                  |

---

## 🧩 Revised “Lab Section” (with refinements)

Here’s the updated *Step 1–4* section with the minor improvements applied:

---

### Step 1 — Generate the PRD

1. Paste the Minimal PRD Prompt into your LLM (ChatGPT, Claude, etc.).
2. Review the generated PRD — note missing sections.
3. Ask the model to help you *fill in the blanks* through iterative prompts.
4. **Save your generated PRD as `docs/PRD.md`.**

### Step 2 — Create Supporting Artifacts
Use prompts like:
* “Create an ADR documenting our first architectural choice (e.g., local vs. hosted storage).”
* “Write a README.md for this project as if it were open source.”
* “List 5 To-Dos the model recommends to make this app usable.”
* “Draft 3 QA assertions that confirm core features are working.”

*(You can stop after Step 2 and still complete the lab successfully.)*


### Step 3 — Prototype It
* Suggest you use **Streamlit** to sketch a minimal UI *or* simply describe the UI in Markdown.
* Display your prompts in a list.
* Add a text box to write or edit one.
* Include a simple export or copy button.

### Step 4 — Reflect
* What did the model assume?
* Where did it hallucinate?
* How could your initial context improve its answers?
* Ask: *“How could I improve this prompt next time?”*

---

## 🚀 Artifact 4 — Advanced Prompt Engineering Steps

**1. Context as Memory**
- Save intermediate prompts and outputs as “context captures.”    
- Compare how output changes as you expand context incrementally.    

**2. Iterative Refinement**
- Ask the model to _review its own PRD_ for completeness.    
- Introduce a “Finished?” check prompt:    
    > “Does this PRD provide enough clarity for an engineer to start coding? If not, what’s missing?”
    

**3. Prompt Versioning**
- Maintain a version number inside each artifact (`v0.1`, `v0.2`, …).    
- Add changelogs describing what was refined in each iteration.    

**4. Chain-of-Thought Exploration**
- Request the model to outline how it reasoned when creating the PRD.    
- Example:    
    > “Summarize the reasoning process you used to decide what sections to include.”
    

**5. Self-Critique Loop**
- Have the model critique its own prompt and improve it.    
- Example:    
    > “Evaluate this prompt’s clarity and specificity using a 1-5 scale. Suggest one better version.”
    

**6. Personalization**
- Tailor Prompt Genius to your own workflow:    
    - Integrate API keys securely.        
    - Store prompt histories locally.        
    - Add categories like _research_, _code_, _summarization_.


---
### License
This Prompt Genius Lab content is released under the **Apache License 2.0**.  
You’re free to use, modify, and share it for educational or commercial purposes, provided attribution is retained and the same license is included.

