## Start a tmux Session To start a new tmux session:

```bash
Copy code
tmux new -s session_name
```

## Detach a tmux Session 
inside
>Ctrl-b d

via Command Line (without being inside it)
```bash
tmux detach-client -s session_name
```

detach all clients
```bash
tmux detach-client -a
```
## Reattach
```bash
tmux attach -t session_name
```

## other
If you don't remember the session name, list the sessions:
```bash
tmux ls
```

Kill the session
```
tmux kill-session -t session_name
```
