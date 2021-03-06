#If you come from bash you might have to change your $PATH.
export PATH=$HOME/bin:/usr/local/bin:$HOME/node_modules/.bin/:$PATH

# Path to your oh-my-zsh installation.
export ZSH="/Users/xueyq/.oh-my-zsh"

# Set name of the theme to load --- if set to "random", it will
# load a random theme each time oh-my-zsh is loaded, in which case,
# to know which specific one was loaded, run: echo $RANDOM_THEME
# See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
ZSH_THEME="robbyrussell"

# Set list of themes to pick from when loading at random
# Setting this variable when ZSH_THEME=random will cause zsh to load
# a theme from this variable instead of looking in ~/.oh-my-zsh/themes/
# If set to an empty array, this variable will have no effect.
# ZSH_THEME_RANDOM_CANDIDATES=( "robbyrussell" "agnoster" )

# Uncomment the following line to use case-sensitive completion.
# CASE_SENSITIVE="true"

# Uncomment the following line to use hyphen-insensitive completion.
# Case-sensitive completion must be off. _ and - will be interchangeable.
# HYPHEN_INSENSITIVE="true"

# Uncomment the following line to disable bi-weekly auto-update checks.
# DISABLE_AUTO_UPDATE="true"

# Uncomment the following line to change how often to auto-update (in days).
# export UPDATE_ZSH_DAYS=13

# Uncomment the following line to disable colors in ls.
# DISABLE_LS_COLORS="true"

# Uncomment the following line to disable auto-setting terminal title.
# DISABLE_AUTO_TITLE="true"

# Uncomment the following line to enable command auto-correction.
# ENABLE_CORRECTION="true"

# Uncomment the following line to display red dots whilst waiting for completion.
# COMPLETION_WAITING_DOTS="true"

# Uncomment the following line if you want to disable marking untracked files
# under VCS as dirty. This makes repository status check for large repositories
# much, much faster.
# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment the following line if you want to change the command execution time
# stamp shown in the history command output.
# You can set one of the optional three formats:
# "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
# or set a custom format using the strftime function format specifications,
# see 'man strftime' for details.
# HIST_STAMPS="mm/dd/yyyy"

# Would you like to use another custom folder than $ZSH/custom?
# ZSH_CUSTOM=/path/to/new-custom-folder

# Which plugins would you like to load?
# Standard plugins can be found in ~/.oh-my-zsh/plugins/*
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
# Add wisely, as too many plugins slow down shell startup.
plugins=(git)

source $ZSH/oh-my-zsh.sh

# User configuration

# export MANPATH="/usr/local/man:$MANPATH"
# You may need to manually set your language environment
# export LANG=en_US.UTF-8

source ~/.bash_profile 

# Preferred editor for local and remote sessions
# if [[ -n $SSH_CONNECTION ]]; then
#   export EDITOR='vim'
# else
#   export EDITOR='mvim'
# fi

# Compilation flags
# export ARCHFLAGS="-arch x86_64"

# ssh
# export SSH_KEY_PATH="~/.ssh/rsa_id"

# Set personal aliases, overriding those provided by oh-my-zsh libs,
# plugins, and themes. Aliases can be placed here, though oh-my-zsh
# users are encouraged to define aliases within the ZSH_CUSTOM folder.
# For a full list of active aliases, run `alias`.
#
# Example aliases
# alias zshconfig="mate ~/.zshrc"
# alias ohmyzsh="mate ~/.oh-my-zsh"

# java home
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-11.0.2.jdk/Contents/Home
#Maven
export M2_HOME=/Library/ApacheMaven
export PATH=$PATH:$M2_HOME/bin

# alias for Application
alias atom='/Applications/Atom.app/Contents/MacOS/Atom'
alias subl='/Applications/SublimeText.app/Contents/SharedSupport/bin/subl'
alias code='/Applications/Visual\ Studio\ Code.app/Contents/Resources/app/bin/code'
#

# Tencent
# alias for proxy
#alias p="http_proxy=http://127.0.0.1:12639 https_proxy=http://127.0.0.1:12639"


# ???????????????????????????
# finder ????????????
alias co='code ./'
alias fo='open ./'

# pod ??? xcode ??????????????????
alias o='open *.xcodeproj'
alias po='open *.xcworkspace'
alias pru='pod repo update'
alias pi='pod install'
alias pu='pod update'
alias piu='pod install --repo-update'
alias repoanalysis='specbackwarddependency /Users/xueyq/.cocoapods/repos/XXCompany_specs'
alias plint='pod lib lint --sources=git@git.***-inc.com:client/App-Specs.git,git@git.***-inc.com:client/CocoaPods-Specs.git --allow-warnings --verbose --use-libraries'
alias errorShow=' >1.log 2>&1'
# git ????????????
alias gck='git checkout'
alias gm='git merge'
alias gb='git branch'
alias gbr='git branch -a'
alias gs='git status'
alias gc='git clone'
alias gl='git log'
alias ga='git add .'
alias gpull='git pull'
alias gpush='git push'
alias gcm='git commit -m'
alias glocalbranchPush='git push --set-upstream origin '
alias glg="git log --graph --pretty=format:'%Cred%h%Crest -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative"
# npm ????????????
alias ns='npm start'
alias ni='npm install'
alias nb='npm run build'
alias nig='npm install -g '
alias nt='npm test'

# Vue ????????????
alias vc='vue-init webpack' # (vue-init webpack test1)?????? vc test1

# React 
alias rc='create-react-app' #(create-react-app todolist)?????? rc todolist

# React Native ??????
alias rnc='react-native init' #(react-native init todolist)?????? rnc todolist


# ????????????????????????
## ???????????????
alias OpenWithSafari='open -a "/Applications/Safari.app" '
alias OpenWithChrome='open -a "/Applications/Google Chrome.app" '
## ??? Typora ?????? markdown ???????????????????????????
alias OpenMDPreview='open -a "/Applications/Typora.app" '
## ??? DB Browser for SQLite ?????? db ??????
alias OpenDB='open -a "/Applications/DB Browser for SQLite.app" '
## ??? SourceTree ????????????
alias openSourceTree='open -a "/Applications/Sourcetree.app/" '
# Flutter ????????????

export PUB_HOSTED_URL=https://pub.flutter-io.cn
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
export PATH=/Users/xueyq/flutter/bin:$PATH


# Android SDK ??????

export ANDROID_HOME=~/Library/Android/sdk
export PATH=${PATH}:${ANDROID_HOME}/emulator
export PATH=${PATH}:${ANDROID_HOME}/tools
export PATH=${PATH}:${ANDROID_HOME}/platform-tools


# iOS ???????????????
alias iOSSimulator='open -a Simulator'

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion


# Node Version Manager
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
# Add RVM to PATH for scripting. Make sure this is the last PATH variable change.
export PATH="$PATH:$HOME/.rvm/bin"

export N_PREFIX=/usr/local/bin/node #??????????????????????????????
export PATH=$N_PREFIX/bin:$PATH
export PATH=/Users/xueyq/Desktop/Github/GitWorkflow/bin:$PATH


# chrome ????????????
# export PATH=/Users/xueyq/Desktop/Tech-Research/iOS/depot_tools:$PATH


# ?????? pyhton ??????
# Setting PATH for Python 2.7
PATH="/System/Library/Frameworks/Python.framework/Versions/2.7/bin:${PATH}"
export PATH
# Setting PATH for Python 3.7.4
PATH="/usr/local/Cellar/python/3.7.4/bin:${PATH}"

alias python='/System/Library/Frameworks/Python.framework/Versions/2.7/bin/python2.7'
alias python3='/usr/local/Cellar/python/3.7.4/bin/python3'



# ?????????????????? homebrew ?????????????????????????????????

alias disableHomebrewUpdate="export HOMEBREW_NO_AUTO_UPDATE=true"


# ??????????????????????????????????????????????????????????????????

function proxy_off(){
    unset ALL_PROXY
    echo -e "???????????????"
}

function proxy_on(){
    export ALL_PROXY=socks5://127.0.0.1:1081
    echo -e "???????????????"
}


# PHP ??????????????????composer
export PATH="~/.composer/vendor/bin:$PATH"

# python ????????????????????????????????? 
export PYENV_ROOT=~/.pyenv
export PATH=$PYENV_ROOT/shims:$PATH


# ??????
# ???????????????????????????????????????
alias showFilesCount='ls -l |grep "^-"|wc -l'