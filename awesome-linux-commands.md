# awesome-linux-commands

## Process

- `pgrep node | xargs kill -9` _Kill all node process_
- `kill -9 $(lsof -t -i:8080)` _Kill any process listening to the port 8080_

## Hardware

- `dmidecode -t memory | grep -i size` _List memory slots_
- `lshw -class memory` _List advanced information about memory slots_
- `echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p` _Increasing the amount of inotify watchers_
