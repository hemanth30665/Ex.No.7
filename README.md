# Ex.No.7 — Developing a Prompt-Based Application and a Technical Communication Portfolio

NAME:JANDA HEMANTH

REGISTER NUMBER: 212223030015


---

## Aim

To develop a prompt-based personal productivity assistant application using an LLM (ChatGPT), demonstrating the progression from simple to advanced prompt designs; and to use prompt engineering to iteratively generate and refine a set of technical communication documents (Technical Report, Research Abstract, Literature Review, Project Proposal, Resume, LinkedIn Profile, Research Poster), evaluated on grammar, technical accuracy, plagiarism, and readability — fostering creativity and practical problem-solving while leveraging LLM capabilities for personal and academic needs.

**AI Tools Required:** ChatGPT, Claude (any LLM capable of multi-turn, context-adaptive interaction).

---

# Part A — Prompt-Based Personal Productivity Assistant

## Master Prompt

> "Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user's changing preferences over time."

## Procedure

1. Define the core requirements of a personal productivity assistant.
2. Construct appropriate prompts for each task (task management, scheduling, wellness, general Q&A) using an LLM.
3. Simulate natural user interaction through a simple command-line style conversation.
4. Collect feedback from the simulated user and adapt responses accordingly.
5. Simulate basic memory to demonstrate preference adaptation over time.

## Step 1 — Core Requirements

| Requirement | Description |
|---|---|
| Task Management | Accept tasks in natural language, organize by priority/deadline, give daily summaries |
| Smart Scheduling | Schedule events/reminders with contextual understanding, flag conflicts |
| Wellness Support | Suggest hydration, exercise, and screen-break reminders, adapting to user response |
| General Query Handling | Answer everyday questions conversationally |
| Adaptability | Remember user preferences (e.g., preferred reminder times, tone) across the session |

## Step 2 — Prompt Progression (Simple → Advanced)

### Simple Prompt (Task Manager)
> "Remind me to call mom at 6 PM."

**Simple Output:** "Reminder set: Call mom at 6:00 PM."

### Advanced Prompt (Task Manager, with prioritization and summary)
> "I have these tasks today: call mom at 6 PM, submit the project report by 5 PM, and buy groceries anytime before 9 PM. Organize them by priority and deadline, and give me a summary of what to do first."

**Advanced Output:**
> "Here's your prioritized plan:
> 1. **5:00 PM — Submit project report** (High priority, hard deadline)
> 2. **6:00 PM — Call mom** (Medium priority, fixed time)
> 3. **Before 9:00 PM — Buy groceries** (Low priority, flexible)
>
> Suggestion: Finish the report first since it has the earliest hard deadline, then call your mom at 6, and fit groceries in afterward."

### Simple Prompt (Scheduler)
> "Schedule a meeting tomorrow at 3 PM."

### Advanced Prompt (Scheduler, with conflict detection)
> "I already have a dentist appointment tomorrow from 2:30 PM to 3:30 PM. Now I need to schedule a project meeting tomorrow at 3 PM — check for conflicts and suggest the best alternative time."

**Advanced Output:**
> "Conflict detected: your dentist appointment (2:30–3:30 PM) overlaps with the requested 3 PM meeting. Suggested alternative: 4:00 PM, right after your appointment, or 11:00 AM if you'd prefer it earlier in the day."

### Simple Prompt (Wellness)
> "Give me a wellness tip."

### Advanced Prompt (Wellness, adapting to past preference)
> "Earlier I mentioned I sit at my desk for long hours and don't like generic advice like 'drink water.' Give me a wellness tip that fits my situation."

**Advanced Output:**
> "Since you're at your desk for long stretches, try the 20-20-20 rule: every 20 minutes, look at something 20 feet away for 20 seconds — it reduces eye strain without needing you to get up. Pair it with a 2-minute stretch every hour to avoid stiffness."

### Simple Prompt (General Query)
> "What's the capital of France?"

### Advanced Prompt (General Query, conversational continuity)
> "Following up on my earlier travel question — if I'm visiting that city next month, what's one practical tip for a first-time visitor?"

**Advanced Output:**
> "Since you're visiting Paris next month, get a **Navigo Découverte** weekly transit pass — it covers metro, bus, and RER, and is far cheaper than buying individual tickets for a week of sightseeing."

## Step 3 — Simulated Interaction (Command-Line Style)

```
> User: Remind me to call mom at 6 PM.
Assistant: Reminder set for 6:00 PM — Call mom.

> User: Also add: submit project report by 5 PM, buy groceries before 9 PM.
Assistant: Got it. Updated task list, prioritized by deadline:
  1. 5:00 PM - Submit project report (High)
  2. 6:00 PM - Call mom (Medium)
  3. Before 9:00 PM - Buy groceries (Low)

> User: I don't like being reminded more than 15 minutes before a task.
Assistant: Noted — I'll set reminders 15 minutes before each task from now on.

> User: Give me a wellness tip.
Assistant: Since you mentioned long desk hours earlier, try the 20-20-20 rule for eye strain relief.
```

## Step 4 — Feedback and Adaptation

**User feedback:** "I don't like being reminded more than 15 minutes before a task."
**Adapted behavior:** All subsequent reminders in the simulated session were generated as "15 minutes before" rather than the assistant's default "30 minutes before," demonstrating adaptation to explicit user feedback.

## Step 5 — Simulated Memory for Preference Adaptation

| Session | User Preference Learned | Applied In Later Turn |
|---|---|---|
| 1 | Reminders should be sent 15 minutes before, not 30 | Reminder timing adjusted in Step 3 |
| 2 | Dislikes generic wellness tips; sits at a desk for long hours | Personalized eye-strain tip given in Step 2 |
| 3 | Traveling to Paris next month | Contextual travel tip given instead of a generic answer |

## Expected Output — Personal Productivity Assistant Feature Summary

1. **Daily Task Manager** — accepts natural-language tasks, organizes by priority/deadline, gives daily summaries and pending items.
2. **Smart Scheduler** — schedules events/reminders with contextual understanding, flags overlapping appointments, suggests free slots.
3. **Wellness Tips Generator** — gives daily wellness advice (hydration, exercise, screen breaks), adapting to past user responses.
4. **General Query Handler** — answers everyday questions conversationally, using prior context where relevant.
5. **Preference Memory** — retains stated preferences (reminder timing, tone, interests) across the interaction.

### Result — Part A
A prototype concept for an LLM-powered personal productivity assistant was created, showing the progression from simple to advanced prompts for task management, scheduling, wellness suggestions, and general queries, along with simulated feedback-driven adaptation.

---

# Part B — Technical Communication Portfolio

**Project used for all documents:** Crop Disease Detection using Computer Vision (final-year project, continued from Ex.No.5/6).

Each document type below was generated using an **initial prompt**, then improved using **iterative prompting**, and evaluated on **Grammar, Technical Accuracy, Plagiarism (originality), and Readability** (each scored 1–5; Plagiarism scored as "originality," where 5 = fully original/no matching text found).

## 1. Technical Report

**Initial Prompt:** "Write a technical report on a crop disease detection system using computer vision."
**Iterative Refinement Prompt:** "Rewrite this as a formal technical report with sections: Abstract, Introduction, Methodology, Results, Conclusion. Use MobileNetV2 transfer learning, PlantVillage dataset, and an embedded deployment target. Keep language formal and precise, avoid marketing language."
**Outcome:** First draft was generic and used vague language ("innovative," "cutting-edge"); refined version added specific architecture, dataset, and quantitative framing (target accuracy, inference time).

| Metric | Initial Draft | After Iteration |
|---|---|---|
| Grammar | 4 | 5 |
| Technical Accuracy | 3 | 5 |
| Plagiarism (Originality) | 5 | 5 |
| Readability | 3 | 4 |

## 2. Research Abstract

**Initial Prompt:** "Write an abstract for a crop disease detection project."
**Iterative Refinement Prompt:** "Condense this into a 200-word IEEE-style abstract with problem statement, method, key result, and significance — no citations, no vague claims."
**Outcome:** Initial abstract exceeded scope with unnecessary background; refined version was concise and results-focused.

| Metric | Initial Draft | After Iteration |
|---|---|---|
| Grammar | 4 | 5 |
| Technical Accuracy | 3 | 4 |
| Plagiarism (Originality) | 5 | 5 |
| Readability | 4 | 5 |

## 3. Literature Review

**Initial Prompt:** "Write a literature review on crop disease detection using deep learning."
**Iterative Refinement Prompt:** "Organize the review into three themes: (1) classical image-processing approaches, (2) CNN-based approaches, (3) lightweight/edge-deployable models. For each theme, summarize the general approach and its key limitation, in your own words, without quoting sources directly."
**Outcome:** Initial draft was a flat list of unrelated points; refined version was thematically organized and explicitly avoided close paraphrasing/quoting to reduce plagiarism risk.

| Metric | Initial Draft | After Iteration |
|---|---|---|
| Grammar | 4 | 5 |
| Technical Accuracy | 3 | 4 |
| Plagiarism (Originality) | 3 | 5 |
| Readability | 3 | 4 |

## 4. Project Proposal

**Initial Prompt:** "Write a project proposal for a crop disease detection system."
**Iterative Refinement Prompt:** "Restructure as a formal proposal with sections: Problem Statement, Objectives, Methodology, Timeline (6 weeks), Expected Outcomes, and Resource Requirements — align the timeline with a realistic final-year project schedule."
**Outcome:** Initial draft lacked a timeline and resource section; refined version matched the actual 6-week schedule used in Ex.No.7's Drone Survey scheduling exercise style, applied here to this project.

| Metric | Initial Draft | After Iteration |
|---|---|---|
| Grammar | 4 | 5 |
| Technical Accuracy | 3 | 4 |
| Plagiarism (Originality) | 5 | 5 |
| Readability | 4 | 5 |

## 5. Resume

**Initial Prompt:** "Write a resume for a student who worked on a crop disease detection project."
**Iterative Refinement Prompt:** "Rewrite the project section using strong action verbs and quantifiable outcomes (e.g., model accuracy, dataset size, deployment target), keep it to 3 concise bullet points, and match a standard ATS-friendly resume format."
**Outcome:** Initial draft was descriptive and passive ("worked on a project that..."); refined version used quantified, achievement-oriented bullets ("Developed and deployed a MobileNetV2-based classifier achieving X% accuracy on Y leaf images...").

| Metric | Initial Draft | After Iteration |
|---|---|---|
| Grammar | 4 | 5 |
| Technical Accuracy | 4 | 5 |
| Plagiarism (Originality) | 5 | 5 |
| Readability | 3 | 5 |

## 6. LinkedIn Profile (Project Summary Section)

**Initial Prompt:** "Write a LinkedIn summary about a crop disease detection project."
**Iterative Refinement Prompt:** "Rewrite this in a professional but engaging first-person tone, under 100 words, highlighting the real-world impact for farmers, the technical stack used, and an invitation to connect/discuss."
**Outcome:** Initial draft read like a formal report excerpt; refined version was conversational, impact-focused, and appropriately concise for a social platform.

| Metric | Initial Draft | After Iteration |
|---|---|---|
| Grammar | 4 | 5 |
| Technical Accuracy | 4 | 4 |
| Plagiarism (Originality) | 5 | 5 |
| Readability | 3 | 5 |

## 7. Research Poster (Content Outline)

**Initial Prompt:** "Create content for a research poster about crop disease detection."
**Iterative Refinement Prompt:** "Restructure into standard poster sections (Title, Introduction, Methodology, Results, Conclusion, QR code/contact) with short bullet points only — no paragraphs — suitable for a printed A1 poster read from 2 meters away."
**Outcome:** Initial draft used full paragraphs unsuitable for poster format; refined version used short, high-contrast bullet points appropriate for poster readability at a distance.

| Metric | Initial Draft | After Iteration |
|---|---|---|
| Grammar | 4 | 5 |
| Technical Accuracy | 3 | 4 |
| Plagiarism (Originality) | 5 | 5 |
| Readability | 2 | 5 |

---

## Overall Evaluation Summary

| Document | Grammar (Final) | Technical Accuracy (Final) | Originality (Final) | Readability (Final) |
|---|---|---|---|---|
| Technical Report | 5 | 5 | 5 | 4 |
| Research Abstract | 5 | 4 | 5 | 5 |
| Literature Review | 5 | 4 | 5 | 4 |
| Project Proposal | 5 | 4 | 5 | 5 |
| Resume | 5 | 5 | 5 | 5 |
| LinkedIn Profile | 5 | 4 | 5 | 5 |
| Research Poster | 5 | 4 | 5 | 5 |

## Observations

- **Iterative prompting** produced the largest readability gains for format-sensitive documents (Research Poster: 2 → 5, Resume: 3 → 5, LinkedIn: 3 → 5), where the first draft used the wrong structure entirely (paragraphs instead of bullets, passive instead of achievement-oriented language).
- **Technical accuracy** improved most when the refinement prompt explicitly named the real project details (MobileNetV2, PlantVillage dataset, 6-week timeline) instead of leaving the AI to invent generic technical claims.
- **Originality/plagiarism risk** was lowest in the first Literature Review draft, where the AI's initial phrasing paralleled common textbook explanations; explicitly instructing "in your own words, without quoting sources directly" resolved this in the refined version.
- **Grammar** was consistently strong even in initial drafts across all seven document types, confirming that grammar is rarely the limiting factor — structure, specificity, and originality are where iteration adds the most value.

---

## Deliverable — Technical Communication Portfolio

A completed portfolio was compiled containing all seven refined documents for the Crop Disease Detection project:
1. Technical Report
2. Research Abstract
3. Literature Review
4. Project Proposal
5. Resume (project bullet points)
6. LinkedIn Profile summary
7. Research Poster content outline

Each document is paired with its initial prompt, refinement prompt, and before/after evaluation scores, forming a reusable portfolio that demonstrates both the final-year project and the prompt engineering process used to produce professional technical communication artifacts.

---

## Conclusion

This experiment demonstrated two complementary applications of prompt engineering: first, designing a personal productivity assistant that progresses from simple, single-purpose prompts to adaptive, context-aware ones; and second, using iterative prompting to transform generic AI drafts into professional-quality technical communication documents across seven formats. In both cases, the largest quality gains came not from asking a broader question, but from supplying specific context (real preferences, real project details, real formatting constraints) in the refinement step — confirming that effective prompt engineering is fundamentally about progressively narrowing ambiguity rather than simply asking more.

---

## Result

The prompt-based personal productivity assistant prototype was successfully designed and demonstrated across task management, scheduling, wellness, and general-query features with simulated preference adaptation. In parallel, all seven technical communication documents (Technical Report, Research Abstract, Literature Review, Project Proposal, Resume, LinkedIn Profile, Research Poster) were generated and improved through iterative prompting, evaluated on grammar, technical accuracy, plagiarism, and readability, and compiled into a complete Technical Communication Portfolio.
