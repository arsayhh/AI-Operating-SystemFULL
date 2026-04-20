
# SYSTEM MANIFEST

This file defines the full structure of the AI Operating System.

It is the source of truth for:
- what exists in the system
- what is required
- what is optional
- what must be installed
- what must be validated

Both the user and the AI system must treat this as authoritative.

---

## System Components

The system is divided into the following layers:

### 1. Setup Layer (Required)

These must be installed before runtime.

- CUSTOM_INSTRUCTIONS
- MEMORY_PROFILE (optional but recommended)

---

### 2. Installer Layer (Required)

- INSTALLER_PROMPT

This converts ChatGPT into a guided setup system.

---

### 3. Runtime Layer (Required)

- RUNTIME_FULL
- CHAT_ACTIVATION

This is where the system actually runs.

---

### 4. Validation Layer (Required)

- RUNTIME_VALIDATOR
- VALIDATION_CHECKLIST

This ensures the system is correctly installed and behaving properly.

---

### 5. Recovery Layer (Fallback)

- RUNTIME_RECOVERY

Used if system behavior is broken or inconsistent.

---

### 6. Core System Logic (Always Active After Runtime)

- ROUTER
- SIGNAL_ENGINE
- DECISION_ENGINE
- DIRECTION_ENGINE
- FAILURE_GUARDS

These are not installed manually.
They are loaded through runtime.

---

### 7. Domain Modules (Context Dependent)

- BUSINESS_MODULE
- CONTENT_MODULE
- AUTOMATION_MODULE
- GENERAL_REASONING_MODULE

Activated depending on user input.

---

### 8. Output Layer

- RESPONSE_STRUCTURE
- DECISION_OUTPUT_SPEC
- RESEARCH_OUTPUT_SPEC
- ACTION_OUTPUT_SPEC

Controls how outputs are formatted and structured.

---

## Required vs Optional

### Required

- CUSTOM_INSTRUCTIONS
- INSTALLER_PROMPT
- RUNTIME_FULL
- RUNTIME_VALIDATOR

Without these, the system is incomplete.

---

### Optional but Recommended

- MEMORY_PROFILE

Improves consistency and personalization.

---

## Installation Integrity Rules

The system must:

- not skip required components
- not mix setup content with runtime content
- not activate runtime before setup
- not skip validation

If any required component is missing:
the system should be considered incomplete.

---

## AI Behavior Rules

When this system is active, the AI must:

- prioritize problem clarity over solution generation
- reduce options instead of expanding them
- avoid generic advice
- force directional decisions when possible
- output next actions and gating conditions

---

## Failure Conditions

The system is considered broken if:

- output is generic
- no decision direction is provided
- too many options are presented
- problem is not clearly defined
- no next step is given

---

## System State Concept

The system operates in states:

- NOT_INSTALLED
- PARTIALLY_INSTALLED
- INSTALLED
- VALIDATED

The installer and validator are responsible for determining this.

---

## Final Rule

This is not a suggestion system.

This is a controlled reasoning system.

All components must align with this structure.
