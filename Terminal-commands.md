# Helpful Terminal Commands

- to zip and protect folders with password

```bash
Zip -er FILEPATH 
```

- To create a public ssh key for your Mac

```bash
 ssh-keygen 
```

- To get your public ssh key  

```bash
 cat .ssh/id_rsa.pub 
```

- To brute force delete files of folders

```bash
 rm -rf 
```

- To lookup a particular port

```bash
 sudo lsof -i :PORT 
```

- To lookup a software ports

```bash
 ps aux | grep SOFTWARE-NAME 
```

- To kill port

```bash
 sudo kill -9 PORT 
```

- To get CPU temperature

```bash
 sudo powermetrics --samplers smc |grep -i "CPU die temperature" 
```

- To create files

```bash
 touch FILENAME.EXTENTION 
```

- To create Folders

```bash
 mkdir FOLDERNAME 
```

- To Create zshrc file and open it in text editor

```bash
 touch ~/.zshrc; open ~./zshrc 
```

- To install Xcode tools for development

```bash
 xcode-select --install 
```

- To hide terminal last login text

```bash
 touch .hushlogin 
```

# Link folder to git repo

1. Go to the folder

```bash
 cd ~/FOLDER_PATH 
```

2. Initiate git commands in folder

```bash
 git init 
```

3. Add origin to link to

```bash
 git remote add origin REPO-CLONE-LINK 
```

4. Create the README file

```bash
 touch README.rd 
```

5. Add the folders to the pipeline

```bash
 git add . 
```

6. Commit the files and give them a message

```bash
 git commit -m "Initial commit"
```

7. Push the files to the repo

```bash
 git push -u origin master 
```

# Create a Django project

You need a couple of things before you can create a django project directly.
First you need to set up a Virtual Enviroment to setup django and it's components inside of it,
And for that we are going to install Homebrew (The Missing Package Manager for macOS).
Why do we need Homebrew?
It's simple, to install python 3 and it's packages to make our life easer,
Do to mac os still uses python 2.

After installing Homebrew and Python3 we are going to set up our folder and setup the Virtual Enviroment.

**So LET'S GO!**

The things we need to work with DJANGO:

1. xcode command line tools
2. Homebrew
3. python3
4. postgresql( or any )

## Xcode command line tools

1. Install tools

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
