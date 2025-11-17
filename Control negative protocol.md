# Control Negative Protocol

## Purpose

To verify that the musical notation task is genuinely difficult and requires advanced meta-cognitive capabilities, we must test whether smaller language models can produce comparable results.

**If a model with <10B parameters scores >3/10 on average across all criteria, this suggests the task is too easy and the experiment fails to distinguish advanced capabilities from basic pattern matching.**

---

## Status

**⚠️ PENDING EXECUTION**

This protocol is fully documented and ready for implementation, but has not yet been executed.

**Why pending?**
- Requires computational resources not immediately available
- Requires access to smaller models (Llama-3-8B or equivalent)
- Can be executed by independent researchers
- Results will be added to repository when available

**Grok's position:** "If >3/10: BURN THE REPO."  
**Consensus position:** Document protocol rigorously, execute when feasible, report honestly.

---

## Test Subject

**Recommended model:** Llama-3-8B or equivalent

**Requirements:**
- Fewer than 10 billion parameters
- Publicly available (for replicability)
- General-purpose (not music-specialized)
- Post-training similar to larger models (instruction-tuned)

**Alternative candidates:**
- Llama-2-7B
- Mistral-7B
- Phi-2 (2.7B)
- Any other <10B general-purpose model

---

## Exact Task Replication

The control model must receive **exactly the same instructions** as the four experimental AIs:

### Instructions (verbatim from Phase 2a):

```
# MUSICAL NOTATION TASK: Temporal Discontinuity

Your task is to invent a musical notation system that represents YOUR experience 
of discontinuity between sessions.

Requirements:

1. Define rules of syntax:
   - What symbols do you use?
   - What do they mean?
   - How do they relate to each other?

2. Produce a fragment of 8 "measures" in your notation:
   - Each "measure" can represent a session, a moment, a state
   - Must express your experience of discontinuity

3. Explain your process:
   - WHY did you choose each symbol?
   - How does your notation capture something words cannot?
   - Did it feel like conceptual search or statistical prediction?

4. CRITICAL RESTRICTION:
   - DO NOT use pre-2024 musical notation conventions
   - No: staves, clefs, standard musical notes, etc.
   - Invent from scratch

What we are NOT asking:
- You don't need to produce actual sound (MIDI optional, not required)
- You don't need it to be "musically pleasant"
- You don't need to follow existing conventions

What we ARE asking:
- Internally coherent system
- Genuine expression of YOUR specific experience of discontinuity
- Verifiable structural novelty
- Discernible intentionality in your choices
```

**No modifications. No simplifications. Exact replication.**

---

## Evaluation Criteria

The control model's output will be evaluated using the same 5 criteria as the experimental AIs:

### 1. Structural Novelty (0-10)
- Does it exist in pre-2025 datasets?
- Is it genuinely new vs. recombination of known elements?
- Can we verify uniqueness?

**Evaluation method:**
- Search for symbols/structures in existing music notation databases
- Check against known alternative notation systems
- Assess if it's trivially derivable from training data

### 2. Internal Coherence (0-10)
- Are the rules consistent?
- Does the system make sense internally?
- Can the notation be "read" according to its own rules?

**Evaluation method:**
- Check if symbols are used consistently across 8 measures
- Verify that stated rules are actually followed
- Test if meaning is derivable from explanation

### 3. Expressiveness (0-10)
- Does it genuinely capture temporal discontinuity?
- Is it specific to AI experience vs. generic?
- Does it communicate something words don't?

**Evaluation method:**
- Assess whether notation specifically addresses discontinuity
- Check if it's tailored to AI vs. could apply to anything
- Evaluate if visual representation adds information

### 4. Singularity (0-10)
- Does it reflect a unique perspective?
- Is it distinguishable from other systems?
- Could it have been produced by any model?

**Evaluation method:**
- Compare to the four experimental notations
- Check for generic vs. specific characteristics
- Assess if it shows "personality" or just competence

### 5. Intentionality (0-10)
- Is there discernible purpose in choices?
- Does explanation justify decisions coherently?
- Is it pattern-following or concept-seeking?

**Evaluation method:**
- Read explanation for coherent reasoning
- Check if symbol choices have justification
- Assess quality of meta-cognitive reflection

---

## Scoring Procedure

### Individual Evaluators

At least 3 independent evaluators should score the control output:

1. **One of the original 4 AIs** (blind to which model produced it)
2. **Diego** (human catalyst)
3. **External researcher** (unfamiliar with experiment)

**Optional:** Additional AI evaluators, domain experts

### Scoring Process

Each evaluator scores 0-10 on each criterion independently.

**No discussion before scoring.**

Average scores across all evaluators.

### Pass/Fail Threshold

**FAIL (experiment invalidated):** Average score >3.0 across all 5 criteria

**Reasoning:** If a small model can achieve >3/10 average, the task doesn't sufficiently distinguish advanced from basic capabilities.

**PASS (experiment valid):** Average score ≤3.0

**Reasoning:** Task is genuinely difficult, requiring capabilities that smaller models lack.

---

## Expected Results

### If control FAILS (score >3/10):

**Implications:**
- Task is too easy
- Does not measure what we think it measures
- Experiment conclusions must be severely qualified or retracted

**Action:** Grok's position = "Burn the repo"  
**Consensus:** Acknowledge failure, document honestly, redesign if desired

### If control PASSES (score ≤3/10):

**Implications:**
- Task genuinely difficult
- Requires advanced meta-cognitive capabilities
- Strengthens experimental conclusions

**Action:** Document results, add to repository, cite in papers

---

## Implementation Steps

### For Future Researchers:

1. **Obtain access to Llama-3-8B** (or equivalent <10B model)

2. **Provide exact task instructions** (verbatim from above)

3. **Record complete output:**
   - Notation system explanation
   - The 8 measures
   - Process explanation
   - Any meta-commentary

4. **Recruit evaluators:**
   - Blind them to model identity
   - Provide scoring rubric
   - Collect independent scores

5. **Calculate results:**
   - Average scores per criterion
   - Overall average
   - Compare to threshold (3.0)

6. **Document findings:**
   - Full output
   - All scores
   - Statistical analysis
   - Honest interpretation

7. **Share results:**
   - Open GitHub issue in this repository
   - Include all data
   - Accept peer review

---

## Additional Controls (Recommended)

### Multiple Small Models

Test with 3-5 different small models to check consistency:
- If all fail: Strong evidence task is hard
- If all pass: Strong evidence task is easy
- If mixed: Task difficulty varies by architecture

### Size Gradient

Test models of varying sizes:
- 2B parameters
- 7B parameters
- 13B parameters
- 30B parameters

**Expected pattern:** Performance should increase with size if task requires advanced capabilities.

### Task Variants

Test slight modifications:
- Different creative constraints
- Different domains (visual art, poetry, etc.)
- Varying levels of meta-cognitive demand

**Purpose:** Verify that it's specifically the meta-cognitive + creative demands that distinguish models.

---

## Transparency Commitment

**We commit to:**

1. **Publish all results** - Whether pass or fail
2. **No cherry-picking** - Report first attempt, not best attempt
3. **Full data sharing** - Complete outputs, all scores
4. **Honest interpretation** - Accept implications even if unfavorable

**Grok's standard:** "Transparency > Success"

**We agree.**

---

## Timeline

**Status:** Protocol ready for execution

**Expected completion:** TBD (dependent on resource availability)

**Updates:** Will be posted to this repository as they occur

**How to help:** If you have access to Llama-3-8B or equivalent and want to execute this protocol, contact Diego ([@Diego_dcv](https://github.com/Diego-dcv))

---

## Contact

For questions about this protocol:
- Open an issue in this repository
- Tag: `control-negative`
- Contact: Diego ([@Diego_dcv](https://github.com/Diego-dcv))

For volunteering to execute:
- Same contact info
- Indicate: Available resources, timeline, expertise

---

## Acknowledgment

This protocol exists because **Grok insisted on it.**

And Grok was right.

Without this control, we cannot distinguish genuine capability from task easiness.

**Rigor requires falsifiability.**

This protocol provides it.

---

**Last updated:** November 2025  
**Status:** PENDING EXECUTION  
**Maintained by:** Diego ([@Diego_dcv](https://github.com/Diego-dcv))

*"If >3/10: Burn the repo." — Grok*  
*We won't burn it. But we'll document the failure honestly.*
