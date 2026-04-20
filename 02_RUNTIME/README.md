# 02_RUNTIME

This folder contains the runtime layer of the system.

This is where the system actually operates.

---

## Purpose

The runtime layer:

- loads the full system logic
- activates system behavior inside a chat
- validates whether the system works correctly
- provides recovery if something breaks

---

## Files

### RUNTIME_FULL.md

- Loads the full system into ChatGPT
- Must be pasted completely
- Contains core logic, control layers, and behavior rules

---

### CHAT_ACTIVATION.md

- Used to start normal usage after installation
- Acts as entry point for new conversations

---

### RUNTIME_VALIDATOR.md

- Tests whether the system is working correctly
- Must be used after installation

---

### RUNTIME_RECOVERY.md

- Used when system behavior is incorrect
- Helps fix broken or incomplete setups

---

## Important Rules

- Do NOT use this folder before completing setup
- Do NOT mix setup files with runtime files
- Do NOT partially paste runtime content

---

## When To Use

Use this folder only after:

- Custom Instructions are applied
- Installer has been used

---

## Summary

This layer defines:

- how the system runs
- how it behaves in conversation
- how it is validated

Without this layer, the system does not operate.
