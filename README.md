# tmux
Terminal Multiplexer

# Tmux arhitecture
```

 #########################################################################################
 #                                                                                       #
 #                      ████████ ███    ███ ██    ██ ██   ██                             #
 #                         ██    ████  ████ ██    ██  ██ ██                              #
 #                         ██    ██ ████ ██ ██    ██   ███                               #
 #                         ██    ██  ██  ██ ██    ██  ██ ██                              #
 #                         ██    ██      ██  ██████  ██   ██                             #
 #                                                                                       #
 #                                                                                       #
 #   *********************************************************************************   #
 #   *                                                                               *   #
 #   *                                    SESSION                                    *   #
 #   *                                                                               *   #
 #   *                                                                               *   #
 #   *   ################################         ################################   *   #
 #   *   #                              #         #                              #   *   #
 #   *   #           WINDOW             #         #           WINDOW             #   *   #
 #   *   #     --------   --------      #         #     --------   --------      #   *   #
 #   *   #     |      |   |      |      #         #     |      |   |      |      #   *   #
 #   *   #     | pane |   | pane |      #         #     | pane |   | pane |      #   *   #
 #   *   #     |      |   |      |      #         #     |      |   |      |      #   *   #
 #   *   #     --------   --------      #         #     --------   --------      #   *   #
 #   *   #                              #         #                              #   *   #
 #   *   #     --------   --------      #         #     --------   --------      #   *   #
 #   *   #     |      |   |      |      #         #     |      |   |      |      #   *   #
 #   *   #     | pane |   | pane |      #         #     | pane |   | pane |      #   *   #
 #   *   #     |      |   |      |      #         #     |      |   |      |      #   *   #
 #   *   #     --------   --------      #         #     --------   --------      #   *   #
 #   *   #                              #         #                              #   *   #
 #   *   ################################         ################################   *   #
 #   *                                                                               *   #
 #   *                                                                               *   #
 #   *                                                                               *   #
 #   *                                                                               *   #
 #   *********************************************************************************   #
 #                                                                                       #
 #                                                                                       #
 #                                                                                       #
 #########################################################################################
```



# Istall
```
sudo apt-get install tmux
```

bash completion [Link1](https://russellparker.me/post/2018/02/16/tmux-bash-autocomplete/) [Link2](https://github.com/imomaliev/tmux-bash-completion/blob/master/completions/tmux) [Link3](https://github.com/Bash-it/bash-it/blob/master/completion/available/tmux.completion.bash)
```
sudo curl https://raw.githubusercontent.com/imomaliev/tmux-bash-completion/master/completions/tmux | sudo tee /etc/bash_completion.d/tmux.sh
```

## List
```
tmux list-sessions
```
```
tmux ls
```

## Attach
```
tmux attach-session -t 5
```

## Rename
usage: rename-session [-t target-session] new-name
```
tmux rename-session -t 4 consul-LAB
```

## Create new
_usage: new-session [-AdDEPX] [-c start-directory] [-F format] [-n window-name] [-s session-name] [-t target-session] [-x width] [-y height] [command]_
```
tmux new session-name docker
```
```
tmux new -s docker
```

## Kill
```
tmux kill-session -t docker
```



