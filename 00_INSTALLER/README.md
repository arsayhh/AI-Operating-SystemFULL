# 00_INSTALLER

This folder contains the installer layer of the system.

Its purpose is to guide setup step by step and prevent incorrect installation.

Do not use these files randomly.
Use them only in the order defined by:

- START_HERE.md
- SYSTEM_MANIFEST.md
- INSTALLATION_FLOW.md

---

## Files in This Folder

### INSTALLER_PROMPT.md
Turns ChatGPT into a guided installer.

### INSTALL_STATE_SCHEMA.md
Defines installation states and what counts as complete.

### VALIDATION_CHECKLIST.md
Provides manual validation criteria after setup.

---

## Important

This folder does NOT contain the runtime system itself.

It contains the installation control layer.

That means:

- it helps you install the system
- it does not replace the runtime
- it should be used before normal operation begins

---

## Rule

If you are not currently installing the system,
do not start here.

Start from:

`START_HERE.md`
