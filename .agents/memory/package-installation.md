---
name: Package installation
description: A Bun package-install callback can interpret a project path as a dependency.
---

Use the existing lockfile and manifest directly when installing project dependencies; passing "." to a package-add operation can add the project itself as a self-dependency.

**Why:** The imported app's package installer accepted "." but temporarily wrote a root package reference into package.json and bun.lock.

**How to apply:** Prefer a lockfile-aware install path for imported projects and inspect package.json/bun.lock after installation for unintended manifest changes.