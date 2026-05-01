## Manual Install

```bash
# Fork from https://github.com/Comfy-Org/ComfyUI
git remote add upstream https://github.com/Comfy-Org/ComfyUI.git # to fetch latest changes from the forked repo
git remote -v
cd ComfyUI

uv venv
uv pip install -r requirements.txt
```

## Update

```bash
git fetch upstream master # original upstream repo uses 'master' as the latest/stable branch
git rebase upstream/master

uv pip install -r requirements.txt
```

## Push Changes

```bash
git push origin master
```

## Start

```bash
uv run main.py
```
