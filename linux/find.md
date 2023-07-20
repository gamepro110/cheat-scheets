---
tags: linux, bash, shell
---

# find

```bash
find {{path}} {{flag arg}}
```

| {{flag arg}} | description                                                                                                             |
|:--------------:| ----------------------------------------------------------------------------------------------------------------------- |
| -type {{arg}}  | d == directory, f == file, l == symbolic link, c == character devices, b == block devices, p == named pipe, s == socket |
| -name {{arg}}  | {{arg}} == name to search for                                                                                           |
| -exec {{cmd}}  | {{cmd}} == bash command to run for each found path. "{}" is placeholder for the found path                              |