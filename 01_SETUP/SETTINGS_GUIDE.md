# SETTINGS GUIDE

This file explains where each setup file must be applied.

Incorrect placement will break the system.

---

## Custom Instructions

File:
- CUSTOM_INSTRUCTIONS.md

Where to place:

ChatGPT → Settings → Custom Instructions / Personalization

Important:

- Do NOT paste this into a normal chat
- This must be saved in settings

---

## Memory Profile

File:
- MEMORY_PROFILE.md

Where to place:

- ChatGPT Memory (if available)
- Or treat as persistent preference context

Important:

- This is NOT a runtime prompt
- Do NOT paste into normal chat unless instructed

---

## Installer Prompt

File:
- 00_INSTALLER/INSTALLER_PROMPT.md

Where to place:

- Paste into a NEW ChatGPT chat as the FIRST message

Purpose:

- Converts ChatGPT into installer mode

---

## Runtime Full

File:
- 02_RUNTIME/RUNTIME_FULL.md

Where to place:

- Paste into the installer chat when instructed

Important:

- Must be pasted completely
- Do NOT mix with setup files

---

## Chat Activation

File:
- 02_RUNTIME/CHAT_ACTIVATION.md

Where to place:

- Used in new chats after installation

---

## Runtime Validator

File:
- 02_RUNTIME/RUNTIME_VALIDATOR.md

Where to place:

- Paste into chat to verify behavior

---

## Common Mistakes

Do NOT:

- paste setup files into runtime chat
- skip installer
- load runtime before setup
- mix multiple files randomly

---

## Summary

Each file has a specific destination.

If you place files incorrectly,
the system will not behave as expected.
