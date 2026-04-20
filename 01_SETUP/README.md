# 01_SETUP

This folder defines how the system is configured at the user level.

These files do NOT belong in normal chat usage.

They are used to configure ChatGPT behavior before runtime.

---

## Files

### CUSTOM_INSTRUCTIONS.md

- Goes into ChatGPT settings
- Defines how the system should behave
- Mandatory for correct operation

---

### MEMORY_PROFILE.md

- Defines persistent user behavior preferences
- Improves consistency across conversations
- Optional but recommended

---

### SETTINGS_GUIDE.md

- Explains where each setup file should be placed
- Prevents incorrect usage

---

## Important Rule

These files are NOT runtime prompts.

Do NOT paste them into a normal chat.

They must be applied in settings or treated as persistent configuration.

---

## When To Use

Use this folder during installation only.

Follow the order defined in:

- START_HERE.md
- INSTALLATION_FLOW.md

---

## Summary

This layer defines:

- how the system thinks
- how it remembers
- how it behaves consistently

Without this layer, runtime will be unstable.
