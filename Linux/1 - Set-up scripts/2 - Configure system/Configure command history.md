ZShell --> fc -lf
- Manual:
	- Add to ~/.zshrc file:
		- setopt SHARE_HISTORY
		- setopt INC_APPEND_HISTORY_TIME
	- Then apply changes
		- source ~/.zshrc
- Script Option:
	- Give the script permissions:
		- sudo chmod +x {script_name}
	- Execute the script with the command SOURCE
		- source {script_name}
```
#!/bin/zsh
if ! grep -q "setopt SHARE_HISTORY" ~/.zshrc; then
    sed -i '1i\setopt SHARE_HISTORY\nsetopt INC_APPEND_HISTORY_TIME' ~/.zshrc
    echo "alias history='fc -lf'" >> ~/.zshrc
fi

source ~/.zshrc
```

Bash --> history
- Add to ~/.bashrc
	- echo 'HISTTIMEFORMAT="%F %T "' >> ~/.bashrc
- Then apply changes
	- source ~/.bashrc