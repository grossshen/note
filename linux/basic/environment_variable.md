# Environment Variable in linux
## file
1. /etc/profile
2. /etc/bashrc
3. ~/.bash\_profile
4. !/.bashrc
profile: login-shell style
bashrc: non-login-shell style
### order
login-shell: /etc/profile -> ~/.profile -> ~/.bashrc -> /etc/bashrc
non-login-shell: ~/.bashrc -> /etc/bashrc
## setting
`source` command to load environment variable immediately
## show
`set`:environment variable of current shell
`env`:environment variable of current user
`export`
`declare`
## Mac OS
settings are simillar
