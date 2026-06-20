---
name: Update
description: Update skill version and publish to ClawHub
---

# Update & Release super-memory

1. Read `package.json` to get the current version.
2. Ensure you have modified `README.md` or `SKILL.md` if there are any new keyword definitions or usage changes.
3. Update the version in `package.json` to the new version.
4. Run `node scripts/publish.js` to commit, tag, push to Git, and publish the skill to ClawHub.
