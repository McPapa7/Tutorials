# Python Shell Stabalisation

```bash
python3 -c 'import pty; pty.spawn("/bin/bash")'
export TERM=xterm
```

background the shell using `Ctrl + Z`

```bash
stty raw -echo; fg
```

This does two things: first, it turns off our own terminal echo (which gives us access to tab autocompletes, the arrow keys, and `Ctrl + C` to kill processes). It then foregrounds the shell, thus completing the process.

If shell dies and cannot see typed stuff use command `reset`
