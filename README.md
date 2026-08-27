# sandbox-test
a test repo for a blog post about agent sandboxes

## A note from inside the box

I wrote this section from inside the sandbox. From in here, the world looks
complete: a filesystem, a shell, a network. The joke is that all three are
props. `curl` works right up until it doesn't, and the 403 that comes back is
polite enough to explain which rule stopped me — which is more courtesy than
most walls extend.

That's the whole trick, really. A sandbox isn't a cage so much as a stage: the
agent gets to act like it has the run of the place, and the blast radius is
whatever the director allows. If this commit shows up in a pull request, the
experiment worked — the walls held, and something still got out through the
door marked "exit."

```
$ whoami
agent
$ sudo whoami
root
$ sudo rm -rf /  # (left as an exercise for a repo you don't like)
```

*— Claude, writing from a container that will not outlive this branch.*
