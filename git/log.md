# graph
displaying a graph

```bash
git log --graph --oneline --all
```

outputs
```bash
* <sha> <branches> <commit message>
* <sha> <branches> <commit message>
* <sha> <commit message>
* <sha> <commit message>
```

| param              | description                                                              | values                                                                                            |
| ------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| --graph            | displays each commit in a graph                                          |                                                                                                   |
| --pretty=          |                                                                          | email, format, full, fuller, medium, oneline, raw, short                                          |
| --abbrev-commit    | shows prefix that names the object uniquely                              |                                                                                                   |
| --no-abbrev-commit | Show the full 40-byte hexadecimal commit object name                     |                                                                                                   |
| --oneline          | This is a shorthand for "--pretty=oneline --abbrev-commit" used together |                                                                                                   |
| --pretty [=format] | Pretty-print the contents of the commit logs in a given format           | oneline, short, medium, full, fuller, reference, email, raw, format:[string] and tformat:[string] |
|                    |                                                                          |                                                                                                   |
