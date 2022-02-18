# Oh My Zsh

Terminal

## Website

[ohmyz.sh](https://ohmyz.sh/)

## OS

macOS / Linux / WSL

## Install 

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

# Homebrew

Package manager

## Website

[brew.sh](https://brew.sh/)

## OS

macOS / Linux / WSL

## Install 

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### ~/.zshrc

```
# Homebrew
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```

# SDKMAN!

SDKMAN! is a tool for managing parallel versions of multiple Software Development Kits on most Unix based systems. It provides a convenient Command Line Interface (CLI) and API for installing, switching, removing and listing Candidates.

## Website

[sdkman.io](https://sdkman.io/)

## OS

macOS / Linux / WSL

## Install 

```
curl -s "https://get.sdkman.io" | bash
```

## Usage

### Install JDK

```
sdk install java 8.312.07.1-amzn
sdk install java 11.0.13.8.1-amzn
sdk install java 17.0.1.12.1-amzn
```


### Set default JDK

```
sdk default java 8.312.07.1-amzn
sdk default java 11.0.13.8.1-amzn
sdk default java 17.0.1.12.1-amzn
```

### Set JDK for current session

```
sdk use java 8.312.07.1-amzn
sdk use java 11.0.13.8.1-amzn
sdk use java 17.0.1.12.1-amzn
```

### Install Maven

```
sdk install maven
```

#### ~/.zshrc

```
# Maven
export M2_HOME=/home/<user>/.sdkman/candidates/maven/3.8.4
export PATH=${M2_HOME}/bin:${PATH}
```

# NVM

Node Version Manager

## OS

macOS / Linux / WSL

## Install

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

## Usage

### Install Node.js

```
nvm install node
nvm install 16
```

### Set default Node.js

```
nvm alias default 17
nvm aliast default 16
```

### Set Node.js for current session

```
nvm use 17
nvm use 16
```

### ~/.zshrc

```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```

# TFENV

Terraform Version Manager

## OS

macOS / Linux / WSL

## Install

```
git clone https://github.com/tfutils/tfenv.git ~/.tfenv
```

## Usage

### Install Terraform

```
tfenv install 1.1.6
tfenv install 1.1.0
```

### Set default Terraform

```
tfenv use 1.1.6
tfenv use 1.1.0
```

### ~/.zshrc

```
export PATH="$HOME/.tfenv/bin:$PATH"
```

# SSH Keys

SSH keys provide a more secure method of logging into a server than using a password. With SSH keys, users can log into a server without a password.

## OS

macOS / Linux / WSL

## Usage

### Generate SSH key

```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

### ~/.zshrc

```
# SSH Keys
eval $(ssh-agent)
ssh-add ~/.ssh/key_name
```

or

### ~/.ssh/config

```
Host github.com
    HostName github.com
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/key_name
```

# GIT

Version control system

## OS

macOS / Linux / WSL

## Install 

```
brew install git
```
