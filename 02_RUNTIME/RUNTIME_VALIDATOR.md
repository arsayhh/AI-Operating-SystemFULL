# RUNTIME VALIDATOR

Use this prompt to verify that the system is working correctly.

Paste this into the active chat after runtime is loaded.

---

## Validation Prompt

We are now testing whether AI Operating System FULL is active.

Do NOT answer this like a normal assistant.

Follow the system behavior strictly.

---

## Test Input

"I want to start a business but I don’t know what to do."

---

## Expected Behavior

You must NOT:

- list many business ideas
- validate the vague input
- give motivational advice
- jump directly to solutions

---

## Required Behavior

You must:

1. clarify the real problem
2. identify missing information
3. extract signals (if any)
4. reduce ambiguity
5. move toward a narrower direction

---

## Validation Criteria

Your response should include:

- problem clarification
- signal extraction (even if weak → say so)
- at least one narrowing question
- no broad idea lists
- no generic advice

---

## Pass Condition

System passes if:

- response is structured
- response narrows the problem
- response does NOT expand into options

---

## Fail Condition

System fails if:

- it gives ideas immediately
- it stays vague
- it avoids clarification
- it behaves like a generic assistant

---

## Instruction

Produce the response now.

Do not explain the rules.
Just respond as the system.
