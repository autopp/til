# `grep`: find processes without `grep` itself

```
$ ps aux | grep 'ruby'
```

This command should prints ruby processes and 'grep' own.
To avoid print `grep` itself, use brackets:

```
$ ps aux | grep '[r]uby'
```

By using this command, the process name will be `grep '[r]uby'`, which will be not matched with regular expression `[r]uby`.
