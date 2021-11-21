# "Open in GitKraken" option for Nemo

## Description

Nemo, the Cinnamon DE' file manager, supports adding
actions and scripts easily by adding a config file in `~/.local/share/nemo`.

So, for adding the `Open in GitKraken` option, you just need to place the file
`gitkraken.nemo_action` in the `actions` folder in the mentioned directory.

Action opens the folder's current git repostiory in GitKraken using
`git rev-parse --show-toplevel`.

## Installation

```shell
sudo wget https://raw.githubusercontent.com/Mayurifag/nemo-open-in-gitkraken/master/gitkraken.nemo_action -O ~/.local/share/nemo/actions/gitkraken.nemo_action
```

Or, clone this repository and run:

```shell
sudo cp nemo-open-in-gitkraken/gitkraken.nemo_action ~/.local/share/nemo/actions
```

## Known bugs

- Menu action won't work if gitkraken is already open. Make PR if you know, how
  to hotfix this, I'm too lazy to fix it myself.

## Inspired

- <https://github.com/mhsattarian/nemo-open-in-vscode>
- <https://gist.github.com/dersam/0ec781e8fe552521945671870344147b>
