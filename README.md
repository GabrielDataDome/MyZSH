# MyZSH

Personal save of my zsh config file

#### To have a clean prompt

vim .oh-my-zsh/themes/agnoster.zsh-theme

In the file make sure this function looks like this, with the comment:

```
# Context: user@hostname (who am I and where am I)
prompt_context() {
  if [[ "$USER" != "$DEFAULT_USER" || -n "$SSH_CLIENT" ]]; then
    #prompt_segment black default "%(!.%{%F{yellow}%}.)%n@%m"
  fi
}
```
