
# INSTALLATION FLOW

This file defines the exact installation sequence.

Do not change the order.
Do not skip steps.
Do not merge steps.

---

## Installation Sequence

### Phase 1 — System Awareness

1. Read:
   - SYSTEM_MANIFEST.md

Goal:
Understand what exists in the system and what is required.

---

### Phase 2 — Setup Layer

2. Apply:
   - 01_SETUP/CUSTOM_INSTRUCTIONS.md

Location:
ChatGPT Settings → Custom Instructions

---

3. Apply:
   - 01_SETUP/MEMORY_PROFILE.md

Location:
Memory / persistent user preferences (if available)

If not available:
Continue, but expect weaker consistency.

---

### Phase 3 — Installer Activation

4. Open:
   - 00_INSTALLER/INSTALLER_PROMPT.md

Action:
- Copy full content
- Paste into a NEW ChatGPT conversation as the FIRST message

Result:
ChatGPT switches into installer mode.

---

### Phase 4 — Guided Installation (inside ChatGPT)

5. Follow installer instructions

The installer must:
- check setup completion
- prevent skipping steps
- guide runtime loading
- track system state

Do not bypass installer logic.

---

### Phase 5 — Runtime Loading

6. Load:
   - 02_RUNTIME/RUNTIME_FULL.md

This loads:
- core system logic
- domain modules
- output rules
- control layers

---

7. Activate:
   - 02_RUNTIME/CHAT_ACTIVATION.md

This prepares normal usage mode.

---

### Phase 6 — Validation

8. Run:
   - 02_RUNTIME/RUNTIME_VALIDATOR.md

Goal:
Confirm system is behaving correctly.

---

9. If validation fails:

Use:
- 02_RUNTIME/RUNTIME_RECOVERY.md

Fix missing or broken components.

---

## Installation Completion Criteria

The system is considered installed only if:

- Custom Instructions applied
- Runtime loaded
- Validator passed

If any of these are missing:
System = NOT READY

---

## Important Rules

- Do not skip phases
- Do not paste setup files into normal chat
- Do not activate runtime before setup
- Do not assume installation is complete without validation

---

## Final State

When installation is complete:

System State = VALIDATED

You can now use the system normally.
