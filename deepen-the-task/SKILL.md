---
name: deepen-the-task
description: Deepen a task or rewrite its prompt using professional practices, primary source material, precise methods, and independent validation. Use when exploring an unfamiliar area, when the user wants more precise language to get better results from an LLM, or asks for a deeper, more rigorous approach without expanding the task.
---

# Deepen the Task

Help the user ask for and perform work they may not yet know how to specify. Improve the method while preserving the intended outcome, deliverable, and constraints.

## Choose the mode

- If the user asks to rewrite or improve a prompt, return the analysis and a self-contained rewritten prompt. Do not execute that prompt.
- If the user asks to deepen or carry out the work, briefly explain the approach and execute it within the authorized scope. A rewritten prompt is optional, not a substitute for doing the work.
- If the user supplies only a task with this skill, apply the deeper approach and carry it out. Respect any request to discuss or plan first.

## Start with four questions

Use this framing as the core of the skill:

> I want a deeper version of this task, not a bigger one. Before rewriting it: (1) say what a top professional in this field would do here that I'm not asking for; (2) name the rawest material they would start from instead of what has already been digested for me; (3) name the specific methods and tools they would use; (4) say what, other than you or me, would show the result is right. Then rewrite my prompt to ask for exactly that.

Answer these concretely for the actual task:

1. **Professional practice:** Identify the consequential omission in the current approach. Describe an action, not an expert persona or a claim to world-class quality.
2. **Source material:** Name the closest useful evidence: original documents, source code, event records, measurements, recordings, specimens, or other primary material. Inspect available material before asking for it; distinguish available sources from needed access.
3. **Methods and tools:** Name the relevant techniques precisely and explain what each would establish. Verify unfamiliar or current technical claims against authoritative sources. Choose tools for their contribution, not their sophistication. Borrow from another discipline only when its method solves a concrete problem here.
4. **Independent validation:** Specify an observable check and what result would count against the conclusion. Prefer appropriate measurements, representative tests, held-out data, reproducible calculations, external standards, or qualified review. Another model's approval alone is not independent evidence. For subjective work, identify audience feedback or explicit criteria and acknowledge what those cannot establish.

## Turn the answers into better work

Use precise domain terminology when it changes the requested operation or makes the result testable. Explain unfamiliar terms briefly so the user can reuse them; do not replace plain language with decorative jargon.

For prompt rewrites, include the intended outcome, available inputs, concrete method, deliverable, constraints, and validation. Make the prompt usable in a new conversation without relying on phrases such as "as discussed above." Do not invent data, access, thresholds, or preferences. State consequential assumptions or ask a focused question when a missing answer prevents a useful rewrite.

For execution, work from the strongest accessible evidence, apply the selected method, and run the validation. Report what was established, what failed or remains uncertain, and any material limitation of the evidence. When ideal sources or tools are unavailable, use a defensible alternative if one exists and explain the limitation. Never imply a check was run when it was only proposed.

## Keep it deeper, not bigger

Prioritize improvements that can change the result. Do not add a research program, elaborate tooling, or additional deliverables merely to signal rigor. Ambitious performance targets are hypotheses to investigate, not facts to insist on despite evidence.

Preserve the user's chosen objective. If the objective itself appears questionable, mention the issue and offer a separate reframing; do not silently substitute a broader assignment. Match the explanation to the task: a small improvement may need only a few sentences before the rewritten prompt or execution.

## Example

For "find out why customers are leaving," distinguish recorded cancellation reasons from behavioral evidence. Define churn and the observation window precisely, inspect appropriately handled account and event records, and choose a cohort analysis or other method suited to the question. Test any claimed predictive signal on later unseen data, and distinguish prediction from causal explanation. Do not promise a causal answer from observational logs alone.

## Origin

The four-question framing is from Felix Rieseberg's [How to be more ambitious: A tutorial for humans with models](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/). This skill adapts it for both prompt rewriting and execution.
