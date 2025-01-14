# ansible-raspberry-pi

Ansible playbook for configuring Raspberry Pi with:
- SSH setup
- ZSH with Oh-My-Zsh
- Neovim as default editor with plugins
- Kitty terminal

## Prerequisites
- Ansible installed on your control machine
- Raspberry Pi with basic OS installed
- SSH access to your Raspberry Pi

## Setup
1. Copy `inventory.template.ini` to `inventory.ini` and update with your Pi's details
2. Run the playbook:
   ```bash
   ansible-playbook -i inventory.ini playbook.yml
   ```

## Features
- Automated Neovim setup with:
  - Vim-Plug plugin manager
  - ALE for linting
  - Git integration with vim-fugitive
  - Text manipulation with vim-surround
