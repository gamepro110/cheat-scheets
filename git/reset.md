---
tags: version-control, cheat-scheet
---

# reset

```bash
git reset [options]
```

| options          | description                                                                     |
| ---------------- | ------------------------------------------------------------------------------- |
| {{path/to/file}} | unstaged specific **file**, if no **file** is provided everything gets unstaged |
| --hard           | throws away any changes and reverts the local back to the remote                |
| --mixed [-N]     |...                                                                             |
| --soft           | keep changes but sets the head to {{Commit}}                                    |
