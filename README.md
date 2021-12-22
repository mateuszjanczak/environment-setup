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

### .zshrc

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

# SSH Keys

SSH keys provide a more secure method of logging into a server than using a password. With SSH keys, users can log into a server without a password.

## OS

macOS / Linux / WSL

## Usage

### Generate SSH key

```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

### .zshrc

```
# SSH Keys
eval $(ssh-agent)
ssh-add ~/.ssh/key_name
```

# GIT

Version control system

## OS

macOS / Linux / WSL

## Install 

```
brew install git
```
