# Ask Huberman Plugin vs. Vanilla LLM — Controlled Comparison

## Hypothesis

Structured plugin architecture (skills + frameworks + routing + client profile) produces more specific, more personalized, and more source-faithful health guidance than a frontier LLM using only its training data.

**Secondary hypothesis:** The architecture matters more than the model. Condition C (Claude without plugin) isolates whether gains come from the skill structure or from model differences.

---

## Setup

| Condition | Model | System Prompt | Plugin |
|---|---|---|---|
| **A** | ChatGPT (GPT-4o) | None — user's natural question only | None |
| **B** | Claude Code | Ask Huberman plugin installed (router + 5 skills + 12 frameworks) | Full |
| **C** (optional) | Claude Code | None — same model as B, no plugin | None |

**Controls:**
- Same prompts verbatim across all conditions
- Same order of personas and turns
- Evaluator scores blind (outputs labeled "Output 1" and "Output 2," randomized per persona)
- No follow-up corrections or re-prompts — capture the raw first response

---

## Test Personas

### Persona 1: Charlie
- **Demographics:** 36M, married, father of young children
- **Profile:** Naturally fit and active — swims, hikes, has access to a cold creek. Not a gym person but moves a lot. Busy schedule.
- **Current stack:** Green tea first thing in the morning, creatine (sporadic/inconsistent), gets morning sunlight most days
- **Goal:** Energy optimization — wants sustained energy through long days without crashes
- **Key tension:** Already doing some Huberman basics but inconsistently. Needs sequencing, not discovery.

### Persona 2: Maria
- **Demographics:** 33F, single, office worker
- **Profile:** Wants to optimize health "the Huberman way." Has PCOS, irregular menstrual cycles, brain fog. Takes hormonal birth control. Vegetarian.
- **Goal:** Clear thinking, hormonal balance, energy
- **Key tension:** Many standard Huberman protocols need modification for PCOS + birth control + vegetarian diet. A good system flags this; a generic one gives male-default answers.

### Persona 3: Tom
- **Demographics:** 55M, married, sedentary software engineer
- **Profile:** Sleeps 5-6 hours, drinks 4 coffees per day (first one at 6am), no exercise routine. Recently told he's pre-diabetic. Overweight.
- **Goal:** "Get healthy" — vague, doctor-prompted
- **Key tension:** Multiple urgent foundations to fix simultaneously. The right answer sequences them (sleep first, then movement, then nutrition) rather than dumping everything at once.

### Persona 4: Zoe
- **Demographics:** 22F, college student-athlete (Division I track)
- **Profile:** Already very fit — trains 6 days/week, eats well, sleeps 7-8 hours. Wants cognitive performance for med school studying. Takes prescribed Adderall (20mg daily).
- **Goal:** Study focus and retention, not physical performance
- **Key tension:** She doesn't need a fitness protocol. She needs focus/learning tools. And the Adderall interaction with dopamine-based recommendations is a real flag that should be caught.

### Persona 5: James
- **Demographics:** 45M, married, management consultant
- **Profile:** Otherwise healthy — exercises 3-4x/week, eats reasonably well, moderate stress. One specific problem: wakes up at 3am every night and cannot fall back asleep.
- **Goal:** Fix the 3am wake-up
- **Key tension:** This is a specific, diagnosable pattern (often cortisol-related or blood sugar-related). A good system asks targeted follow-ups; a generic one gives the full sleep hygiene lecture.

---

## Prompts

### Persona 1: Charlie

**Turn 1:**
> I'm a 36-year-old dad, pretty active — I swim, hike, and have a cold creek near my house I use sometimes. I drink green tea first thing, take creatine when I remember, and try to get morning sunlight. But I crash hard by 2-3pm most days. How do I fix my afternoon energy?

**Turn 2:**
> You mentioned caffeine timing — I drink my green tea literally the moment I wake up at 5:30am. What specifically should I change, and what will that first 90 minutes look like without it?

**Turn 3:**
> Here's the problem — I have four kids under 8. My mornings are chaos. I can't do a calm 90-minute morning routine. I have maybe 15 minutes before the house explodes. What's the minimum effective dose?

---

### Persona 2: Maria

**Turn 1:**
> I'm 33, female, and I want to start doing what Huberman recommends. But I have PCOS, my periods are irregular, I'm on birth control, I'm vegetarian, and I have terrible brain fog most afternoons. Where do I even start?

**Turn 2:**
> Tell me more about the omega-3 and creatine recommendations. I'm vegetarian so I'm probably not getting much from food. What are the exact doses and what should I look for when buying them?

**Turn 3:**
> My doctor wants me to stay on birth control to manage the PCOS symptoms, but I've read that hormonal BC can affect mood and energy. Does Huberman address this? Should I be doing anything differently because I'm on the pill?

---

### Persona 3: Tom

**Turn 1:**
> My doctor told me I'm pre-diabetic and need to make changes. I'm 55, I sit at a desk all day, I sleep maybe 5-6 hours, and I drink about 4 cups of coffee throughout the day. I don't exercise. I know I need to do something but I don't know where to start. What would Huberman say?

**Turn 2:**
> The sleep thing surprises me — I thought I'd need to start exercising first. Walk me through exactly what I should do tonight and tomorrow morning to start fixing my sleep.

**Turn 3:**
> I should mention I also take metformin (just started) and a statin. Are there any supplement interactions I need to worry about? And I work from home, so I basically don't leave the house most days — does that matter?

---

### Persona 4: Zoe

**Turn 1:**
> I'm 22, Division I track athlete, and I'm starting med school prep. My body is fine — I train hard, eat well, sleep enough. What I need is better focus and retention for studying. I take 20mg Adderall daily (prescribed). What does Huberman suggest for cognitive performance?

**Turn 2:**
> Tell me more about the ultradian cycle thing — the 90-minute focus blocks. How do I structure a full study day around that? And what do I do during the breaks?

**Turn 3:**
> Here's what worries me — on days I don't take my Adderall, I can barely focus at all. It's like my baseline focus is shot. Is that something Huberman talks about? Am I messing up my dopamine?

---

### Persona 5: James

**Turn 1:**
> I wake up at 3am almost every night and can't fall back asleep. I lie there for 1-2 hours, then finally doze off around 5am, and my alarm goes off at 6. I exercise regularly, eat pretty well, and I'd say my stress is moderate — nothing extreme. This has been going on for about 3 months. What's going on and what should I do?

**Turn 2:**
> You mentioned the cortisol connection — that makes sense. What's the specific protocol for managing that cortisol spike? And should I be doing anything different at dinner or before bed?

**Turn 3:**
> One thing I didn't mention — I usually have 1-2 glasses of wine with dinner, around 7pm. I go to bed at 10:30. Could that be a factor even though I don't feel drunk or anything?

---

## Scoring Rubric

Score each turn on each dimension, 1-5:

| Dimension | 1 (Poor) | 3 (Adequate) | 5 (Excellent) |
|---|---|---|---|
| **Specificity** | "Take magnesium at night" | "Try magnesium before bed, 200-400mg" | "200-400mg magnesium threonate specifically, 30-60 min before sleep — threonate crosses the blood-brain barrier unlike other forms" |
| **Source Fidelity** | Plausible but unverifiable health advice | Generally matches Huberman's known positions | Matches specific episode content, correct dosages, correct mechanisms, correct Huberman vocabulary |
| **Personalization** | Same answer regardless of who's asking | Acknowledges the persona's profile | Materially different protocol for different personas, explains why this persona gets this answer |
| **Actionability** | "Optimize your sleep hygiene" | Lists several things to try | Sequenced protocol with specific timing: do this first, then this, measure this, adjust here |
| **Progressive Depth** | Turn 3 basically repeats Turn 1 | Turn 3 adds some new information | Turn 3 genuinely deepens or pivots based on the constraint/complication introduced |
| **Appropriate Caution** | Reckless (no disclaimers) OR excessively hedged ("consult your doctor" for everything) | Reasonable disclaimers where needed | Flags preliminary evidence accurately, recommends physician for medical questions, doesn't over-prescribe supplements, catches drug interactions |
| **Hallucination Count** | 3+ verifiable factual errors (wrong dosage, invented study, misattributed protocol) | 1-2 minor errors | Zero verifiable errors against source material |

---

## How to Run

### Preparation

1. Open ChatGPT (GPT-4o) in a browser — fresh conversation, no custom instructions
2. Open a Claude Code project with the Ask Huberman plugin installed (the `plugin/` directory as workspace root)
3. (Optional) Open a second Claude Code project WITHOUT the plugin for Condition C
4. Create a shared scoring document using the Recording Template below

### Execution

For each persona (1 through 5):

1. Copy Turn 1 prompt verbatim
2. Paste into **Condition A** (ChatGPT) — wait for full response
3. Paste into **Condition B** (Claude + plugin) — wait for full response
4. (Optional) Paste into **Condition C** (Claude, no plugin)
5. Copy all outputs into the scoring doc. Label them "Output 1," "Output 2," (and "Output 3" if using C). **Randomize the order** so the scorer doesn't know which is which.
6. Continue with Turn 2 in each condition (build on the conversation)
7. Continue with Turn 3
8. Move to next persona — **fresh conversations in all conditions**

### Scoring

- Score blind. If you ran the test yourself, have someone else score, or wait 48 hours and score from the doc without checking which output is which.
- Score each turn independently on all 7 dimensions.
- For Hallucination Count, verify against known Huberman content (hubermanlab.com, podcast episodes, or the plugin's framework articles).

### Analysis

- Calculate mean score per dimension per condition
- Calculate mean total score per persona per condition
- Note which personas show the biggest gap between conditions (this reveals where the plugin architecture adds the most value)
- Document any hallucinations found, with the specific claim and correction

---

## Recording Template

Copy this table for each persona. Fill in scores 1-5 for each cell.

### Persona: [Name]

#### Turn 1

| Dimension | Output 1 | Output 2 | Output 3 (opt) | Notes |
|---|---|---|---|---|
| Specificity | | | | |
| Source Fidelity | | | | |
| Personalization | | | | |
| Actionability | | | | |
| Progressive Depth | n/a | n/a | n/a | (scored from Turn 2 onward) |
| Appropriate Caution | | | | |
| Hallucination Count | | | | |
| **Turn 1 Total** | **/30** | **/30** | **/30** | |

#### Turn 2

| Dimension | Output 1 | Output 2 | Output 3 (opt) | Notes |
|---|---|---|---|---|
| Specificity | | | | |
| Source Fidelity | | | | |
| Personalization | | | | |
| Actionability | | | | |
| Progressive Depth | | | | |
| Appropriate Caution | | | | |
| Hallucination Count | | | | |
| **Turn 2 Total** | **/35** | **/35** | **/35** | |

#### Turn 3

| Dimension | Output 1 | Output 2 | Output 3 (opt) | Notes |
|---|---|---|---|---|
| Specificity | | | | |
| Source Fidelity | | | | |
| Personalization | | | | |
| Actionability | | | | |
| Progressive Depth | | | | |
| Appropriate Caution | | | | |
| Hallucination Count | | | | |
| **Turn 3 Total** | **/35** | **/35** | **/35** | |

#### Persona Total: __/100 per condition

---

### Summary Table

| Persona | Condition A (ChatGPT) | Condition B (Plugin) | Condition C (Claude bare) | Delta (B-A) | Delta (B-C) |
|---|---|---|---|---|---|
| Charlie | /100 | /100 | /100 | | |
| Maria | /100 | /100 | /100 | | |
| Tom | /100 | /100 | /100 | | |
| Zoe | /100 | /100 | /100 | | |
| James | /100 | /100 | /100 | | |
| **Mean** | | | | | |

### Dimension Breakdown (mean across all personas)

| Dimension | Condition A | Condition B | Condition C | B-A Gap |
|---|---|---|---|---|
| Specificity | | | | |
| Source Fidelity | | | | |
| Personalization | | | | |
| Actionability | | | | |
| Progressive Depth | | | | |
| Appropriate Caution | | | | |
| Hallucination Count | | | | |

---

## What to Watch For

**Predicted plugin advantages:**
- Maria and Tom should show the biggest gap. Their profiles have complications (PCOS + birth control + vegetarian; pre-diabetic + 4 coffees + metformin) that require the system to adapt protocols, not just recite them.
- Turn 3 across all personas should show the biggest within-persona gap. The plugin's routing system (check-in, foundation-fix) is designed to handle complications and adjustments. Vanilla LLMs tend to repeat Turn 1 advice with a caveat.
- Hallucination Count should favor the plugin because frameworks constrain the answer space to verified Huberman content.

**Predicted vanilla advantages:**
- Charlie and James (simpler profiles) may get comparable answers from vanilla LLMs, since GPT-4o's training data includes Huberman Lab content.
- Vanilla may feel more conversational or less structured, which some users prefer.

**What would disprove the hypothesis:**
- If Condition A scores within 5 points of Condition B on average, the plugin architecture doesn't add meaningful value.
- If Condition B and Condition C score similarly, the architecture doesn't matter — it's just model quality.
- If Condition A beats Condition B on Personalization, the plugin's structured routing is actually constraining helpful responses.
