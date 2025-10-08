# my.bashrc
HISTCONTROL=ignoreboth
 HISTSIZE=100000
 HISTFILESIZE=100000
 HISTTIMEFORMAT='[%F %T] '
 HISTIGNORE="history:history :ls:ll:ls -la"
 PROMPT_COMMAND='history -a; history -c; history -r'
 LESSHISTFILE="-"
 #export PS1='\[\e[0;33m\]#\D{%Y/%m/%d %H:%M:%S} \[\e[0;32m\]@\H:\[\e[1;31m\]\w \n\[\e[1;31m\]#\u\[\e[1;37m\]\$'
 #export PS1='#\D{%Y/%m/%d %H:%M:%S} @\H:\w \n#\u\$ '
 export PS1='#\u@\H:\w \n#\$ '
 export RSYNC_RSH=ssh
 alias ls='ls -CF'
 alias ll='ls -lFh --show-control-chars --color=auto'
 alias mv='mv -iv'
 alias rm='rm -iv'
 alias rmdir='rmdir -v'
 alias cp='cp -iv'
 alias chmod='chmod -v'
 alias chown='chown -v'
 alias mkdir='mkdir -v'
 alias cd='pushd'
 alias less='less -FMRX'
 alias ps='ps --sort=start_time'
 #alias vi='vim'
 alias ln='ln -v'
# alias ansible='ansible -v'
# alias ansible-playbook='ansible-playbook -v'
 alias curl='curl -sSkL'
 alias wget='wget --no-check-certificate'
 alias diff='diff -sup'
 shopt -s autocd
 shopt -s cdspell
 shopt -s direxpand
 shopt -s dirspell
 shopt -s globstar
 shopt -s xpg_echo
 shopt -s checkwinsize
 shopt -s histappend
 shopt -s histverify
 shopt -s histreedit
 shopt -s checkhash
 shopt -s cmdhist
 alias cls='clear'
# alias timestamp='date '+%Y%m%d-%H%M%S''
# #export http_proxy=http://localhost:8080
# #export https_proxy=http://localhost:8080