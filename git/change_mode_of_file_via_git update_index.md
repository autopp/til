# Change mode of file via `git update-index`

Normally, when changing the mode of the file in the repository, execute the following command:

```
$ chmod a+x filename
$ git add filename
```

This can also done with the following `git update-index` command:

```
$ git update-index --add --chmod=+x filename
```

The letter is useful when using Git on Windows.
