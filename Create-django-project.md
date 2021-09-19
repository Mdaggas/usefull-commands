# Create a Django project

You need a couple of things before you can create a django project directly.
First you need to set up a Virtual Enviroment to setup django and it's components inside of it,
And for that we are going to install Homebrew (The Missing Package Manager for macOS).
Why do we need Homebrew?
It's simple, to install python 3 and it's packages to make our life easer,
Do to mac os still uses python 2.

After installing Homebrew and Python3 we are going to set up our folder and setup the Virtual Enviroment.

**So LET'S GO!**

## The things we need to work with DJANGO

1. xcode command line tools
2. Homebrew
3. python3
4. postgresql(or any database)

## Xcode command line tools

- Install tools

```bash
 xcode-select --install 
```

## Homebrew

1. Install Homebrew in your Terminal

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Check Homebrew version

```bash
 brew --version
```

## Python3

1. Install Python3 in your Terminal

```bash
brew install python
```

2. Check python version

```bash
 python3 --version
```

## Postgresql database

You can install Postgresql in two diffrenet ways, you can install there GUI App or a terminal Package with homebrew.

### GUI App installation ***preferred***

- Go to <https://postgresapp.com/downloads.html> and download the lateset version.
