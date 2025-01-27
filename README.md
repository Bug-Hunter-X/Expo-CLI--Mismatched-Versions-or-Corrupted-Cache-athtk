# Expo CLI: Version Mismatch or Corrupted Cache

This repository demonstrates a common issue encountered with the Expo CLI: build failures due to version mismatches or corrupted local cache. The `bug.js` file represents a simple Expo app where the error may manifest. The solution involves resolving version conflicts and clearing the cache.

## Problem

The primary cause is often a discrepancy between the globally installed Expo CLI and the version your project expects.  Corrupted cache files can also lead to inconsistent behavior.

## Solution

1. **Check Expo CLI Version:** Verify the version installed globally using `expo --version`.  Compare this with the Expo version specified in your project's `package.json` (look for `expo` in the `dependencies` section).
2. **Clear Expo Cache:** Run `expo cache:clear` to remove potentially corrupted cache entries.
3. **Reinstall Expo CLI:** If necessary, uninstall and reinstall the Expo CLI: `npm uninstall -g expo-cli` followed by `npm install -g expo-cli`.
4. **Check project dependencies:** Ensure all project dependencies are correctly installed and updated: `npm install` or `yarn install`