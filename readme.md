### Configuração de ambiente

## ZSH

- https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH

## OHMYZSH

- https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh
## GNOME
- sudo apt-get install dconf-cli

- git clone https://github.com/dracula/gnome-terminal

- cd gnome-terminal

- ./install.sh

## Fira Code 
- https://github.com/tonsky/FiraCode/releases

## Tema Terminal
- git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"

- ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

    SPACESHIP_PROMPT_ORDER=(
        user          # Username section
        dir           # Current directory section
        host          # Hostname section
        git           # Git section (git_branch + git_status)
        hg            # Mercurial section (hg_branch  + hg_status)
        exec_time     # Execution time
        line_sep      # Line break
        vi_mode       # Vi-mode indicator
        jobs          # Background jobs indicator
        exit_code     # Exit code section
        char          # Prompt character
    )
    SPACESHIP_USER_SHOW=always
    SPACESHIP_PROMPT_ADD_NEWLINE=false
    SPACESHIP_CHAR_SUFFIX=" "
# Plugins
- sh -c "$(curl -fsSL https://raw.githubusercontent.com/zdharma/zinit/master/doc/install.sh)"

## -
    zinit light zdharma/fast-syntax-highlighting
    zinit light zsh-users/zsh-autosuggestions
    zinit light zsh-users/zsh-completions