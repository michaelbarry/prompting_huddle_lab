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

### Step 1 — Generate the PRD

1. Paste the Minimal PRD Prompt into your LLM (ChatGPT, Claude, etc.).
    
2. Review the generated PRD — note missing sections.
    
3. Ask the model to help you _fill in the blanks_ through iterative prompts.
    

### Step 2 — Create Supporting Artifacts

Use prompts like:

- “Create an ADR documenting our first architectural choice.”
    
- “Write a README.md for this project as if it were open source.”
    
- “List 5 To-Dos the model recommends to make this app usable.”
    
- “Draft 3 QA assertions that confirm core features are working.”
    

### Step 3 — Prototype It

- Use **Streamlit** to sketch a minimal UI.
    
- Display your prompts in a list.
    
- Add a text box to write or edit one.
    
- Include a simple export or copy button.
    

### Step 4 — Reflect

- What did the model assume?
    
- Where did it hallucinate?
    
- How could your initial context improve its answers?
    

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

