Today I've learnt a new git command: `git stash`. It gives you the ablility to save your changes temporarily without committing them. It's like a clipboard for your changes. You can save your changes and then restore them later.

## Tutorial

https://www.youtube.com/watch?v=DeU6opFU_zw&ab_channel=Academind

<iframe width="560" height="315" src="https://www.youtube.com/embed/DeU6opFU_zw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## How to use `git stash`

### Stash your changes

```bash
git stash
```

### List your stashes

```bash
git stash list
```

### stash staged and unstaged changes

```bash
git stash -u
```


### Restore your stashes

```bash
git stash pop
```

### Delete your stashes

```bash
git stash drop
```

### Stash your changes with a message

```bash
git stash save "your message"
```

