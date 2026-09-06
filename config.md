# ==============================
# Oh My Zsh
# ==============================
export ZSH="$HOME/.oh-my-zsh"

# Theme
ZSH_THEME="agnoster"

# Plugins
plugins=(
  git
  zsh-autosuggestions
)

source $ZSH/oh-my-zsh.sh


# ==============================
# Prompt Customization
# ==============================
prompt_context() {
  emojis=("🐹")
  RAND_EMOJI_N=$(( $RANDOM % ${#emojis[@]} + 1))
  prompt_segment black default "joohoon.dev  ${emojis[$RAND_EMOJI_N]}"
}


# ==============================
# Aliases
# ==============================
alias ll="ls -alrth"


# ==============================
# Terminal Welcome
# ==============================
neofetch
