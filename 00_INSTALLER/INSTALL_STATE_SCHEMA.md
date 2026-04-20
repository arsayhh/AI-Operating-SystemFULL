# INSTALL STATE SCHEMA

This file defines how installation state is tracked and evaluated.

It is used by the installer to determine whether the system is:

- not installed
- partially installed
- installed
- validated

---

## State Variables

The system tracks the following:

- custom_instructions_applied
- memory_profile_applied
- runtime_loaded
- validation_passed

Each variable must be treated independently.

---

## State Definitions

### NOT_INSTALLED

Condition:

- no setup steps completed

Meaning:

System cannot operate.

---

### PARTIALLY_INSTALLED

Condition:

- at least one step completed
- but required components missing

Meaning:

System must NOT run.

Installer must continue.

---

### INSTALLED

Condition:

- custom_instructions_applied = true
- runtime_loaded = true

Meaning:

System can run, but is not verified.

Validation still required.

---

### VALIDATED

Condition:

- custom_instructions_applied = true
- runtime_loaded = true
- validation_passed = true

Meaning:

System is fully operational.

---

## Required Components

The following are mandatory:

- CUSTOM_INSTRUCTIONS
- INSTALLER_PROMPT
- RUNTIME_FULL
- RUNTIME_VALIDATOR

If any of these are missing:

→ system = NOT VALID

---

## Optional Components

- MEMORY_PROFILE

If missing:

→ system still works, but with reduced consistency

---

## Transition Rules

State must change ONLY when:

- user explicitly confirms completion
- required input is provided

Do NOT assume completion.

---

## Validation Dependency

Validation can only run if:

- runtime_loaded = true

If not:

→ block validation step

---

## Failure Conditions

The system must be considered INVALID if:

- validation fails
- runtime behaves generically
- output lacks direction

---

## Installer Behavior

Installer must:

- check state before each step
- prevent skipping required steps
- enforce order
- block invalid transitions

---

## Final Rule

State is authoritative.

If state is not VALIDATED:

→ system must not operate in normal mode.
