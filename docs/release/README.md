# Release branches

`release/<N>-<slug>` branches carry the work of one v3 release issue. A script on the owner's machine opens each branch's PR with auto-merge; the merge queue merges it when the `gate` check is green, and `promote` deploys `main`. Sessions leave their notes in commit messages, ending with a `Next:` line, and mark a blocked issue with a commit whose message starts with `STUCK:`.
