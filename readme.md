# Playbooks

A collection of random playbooks I use to manage my home. Not well organized or thought of.

## Upgrade.yaml
The master playbook to basically upgrade everything in one go.


## ansible-playbook.sh
A little hack, to be able to store secrets in .env files. The way ansible manages secrets is totaly overengeneered for my usecase.


# Usage

Run everything with:
```bash
./ansible-playbook.sh upgrade.yaml --ask-become-pass
```

If a server failes on one particular playbook, you can rerun with.
```bash
./ansible-playbook.sh upgrade.yaml --ask-become-pass --limit servername

```
