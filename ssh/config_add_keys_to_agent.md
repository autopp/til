# `.ssh/config`: `AddKeysToAgent` for omitting manual key addition

To use agent forwarding, the key should be registered to ssh-agent via:

```
$ ssh-add ~/.ssh/id_rsa
```

This command needs to be executed every time the OS is rebooted.
You can omit this manual work by adding the following setting to `~/.ssh/config`:

```
# Apply to all host
Host *
  AddKeysToAgent yes
```

With this setting, `ssh` automatically registers the read key in ssh-agent.
