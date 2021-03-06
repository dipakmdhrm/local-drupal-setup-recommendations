# Shell config:
- Terminal Emulator: Terminal, iterm
- Shell application: Bash, Zsh, Fish
## Choosing a shell
### Bash:
  - Most basic and popular shell.
  - Default shell in most Linux OSes and MacOS upto Mojave
  - **Pros:**
    - Basic and easy to use.
    - Plugin support via oh-my-bash:
  - **Cons:**
    - Feature-less
  - **Recommended for:**
    - Basic shell use
### Zsh
  - Default shell in MacOS Catalina
  - **Pros:**
    - Default color coding
    - Automatic cd
    - Plugin support via oh-my-zsh:
      - Themes
      - Autocomplete
  - **Cons:**
    - A little tricky to setup.
  - **Installation instructions:**
    - Comes preinstalled, just switch shell by running:
      - `chsh -s $(which zsh)`
    - Install oh-my-zsh by running:
      - `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
  - **Recommended for:**
    - Devs used to Bash
    - Devs working with a lot of existing scripts and aliases
### Fish
  - New 'exotic shell'
  - **Pros:**
    - Default autocompletion
    - Real-time command syntax highliting
    - Plugin support via oh-my-zsh:
      - Themes
  - **Cons:**
    - Has it's own language
      - Means, you'll need to convert all your alias and scripts to FISH.
  - **Installation:**
    - Install via brew:
      - `brew install fish`
      - Set as default:
        - Add `/usr/local/bin/fish ` to `/etc/shells`:
          - `echo /usr/local/bin/fish | sudo tee -a /etc/shells`
        - `chsh -s /usr/local/bin/fish`
      - Install oh-my-fish:
        - `curl -L https://get.oh-my.fish | fish`
        - Install oh-my-fish plugins:
          - `omf install [name]`
            - Example: `omf install agnoster`
        - Change theme:
          - `omf theme [name]`
            - Example: `omf theme agnoster`
  - **Recommended for:**
    - Everyone who is currently not working with a lot of existing scripts and aliases
