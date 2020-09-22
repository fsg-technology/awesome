# Tips and Tricks: git

To ignore a file without adding it to the ``.gitignore`` file.

```bash
$ git update-index --assume-unchanged config/database.yml
```

To revert back

```bash
$ git update-index --no-assume-unchanged config/database.yml
```

To show a list of ignored files

```bash
 $ git ls-files -v | grep '^h '
 
 h config/database.yml
```

[Source Reference](https://stackoverflow.com/questions/6791889/git-untrack-a-file-in-local-repo-only-and-keep-it-in-the-remote-repo/6793752#6793752)



