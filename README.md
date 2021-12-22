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
