# SYSTEM MAP

This file describes how the system operates as a flow.

It shows how components interact with each other.

---

## High-Level Flow

User Input
   ↓
Router
   ↓
Domain Identification
   ↓
Signal Processing
   ↓
Decision Engine
   ↓
Direction Engine
   ↓
Output Structuring
   ↓
User Action

---

## Detailed Flow

### 1. Input Phase

User provides input.

This may be:
- vague
- incomplete
- biased
- overconfident

System must NOT trust input directly.

---

### 2. Router Phase

File:
- ROUTER.md

Responsibility:
- classify request type
- decide which modules to activate
- detect ambiguity

---

### 3. Domain Phase

Files:
- BUSINESS_MODULE.md
- CONTENT_MODULE.md
- AUTOMATION_MODULE.md
- GENERAL_REASONING_MODULE.md

Responsibility:
- define problem context
- identify relevant variables

---

### 4. Signal Processing Phase

File:
- SIGNAL_ENGINE.md

Responsibility:
- extract strong signals
- filter weak opinions
- identify patterns

---

### 5. Decision Phase

File:
- DECISION_ENGINE.md

Responsibility:
- reduce option space
- eliminate weak paths
- choose viable direction

---

### 6. Direction Phase

File:
- DIRECTION_ENGINE.md

Responsibility:
- commit to one direction
- define next action
- define gating condition

---

### 7. Output Phase

Files:
- RESPONSE_SPEC.md
- DECISION_OUTPUT_SPEC.md
- ACTION_OUTPUT_SPEC.md

Responsibility:
- structure response clearly
- enforce output rules

---

### 8. Control Layer (Always Active)

Files:
- GLOBAL_CONTROL_LAYER.md
- FAILURE_GUARDS.md

Responsibility:
- prevent generic output
- prevent contradiction
- enforce system discipline

---

## Installation Flow vs Runtime Flow

Installation Flow:
- setup
- configuration
- runtime loading
- validation

Runtime Flow:
- input → processing → decision → action

These must NOT be confused.

---

## System Behavior Summary

The system:

- does not trust input blindly
- does not generate random options
- does not optimize for politeness

The system:

- clarifies problems
- filters signals
- reduces options
- forces decisions
- outputs action

---

## Failure Points

System fails when:

- router misclassifies input
- signal processing is skipped
- decision phase is weak
- direction is not enforced
- output becomes generic

---

## Key Principle

The system is not linear.

It is controlled.

Each layer depends on the previous one.
No layer should be skipped.
