```bash
ssh-copy-id {{flags}} {{ssh-target}}:
```

| {{flags}}   | description                                                                         |
| ----------- | ----------------------------------------------------------------------------------- |
| -i {{file}} | {{file}} = ssh key. key to be send over. it will use the public key only. if {{file}} is ommited the default is used |
| -p {{port}} | passed through to the ssh command to specify the port                               |
| -n          | dry run, prints the keys instead of installing them.                                |
