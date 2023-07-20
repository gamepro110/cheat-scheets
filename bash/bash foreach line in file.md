---
tags: linux, shell, scripting
---

# bash foreach line in file

for each line $i in `file` do `cmd $i`, sleep for 1 Ms.

```bash
for i in $(cat <file>); do <cmd> $i; sleep 1; done
```
