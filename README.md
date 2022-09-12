# Setup for Internet Computer Web3 Development

<i>OS: Windows 10</i>

## Install WSL Ubuntu

Open PowerShell as Administrator and run:
```
wsl --install -d Ubuntu
```

<i>Next steps will be executed in the ubuntu terminal.</i>
## Install Homebrew (Package Manager)

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Execute the steps shown after the homebrew installation.

## Install NodeJS

```
brew install node
```

## Install Internet Computer SDK (DFINITY)
```
sh -ci "$(curl -fsSL https://internetcomputer.org/install.sh)"
```

## Set PATH
``` 
export PATH=$PATH:<REPLACE_FOR_DFX_BIN_PATH>
```
Something like this -> /home/your_username/bin

## Create new DApp
```
dfx new hello_world
```

## Deploy 
First terminal, run:
```
dfx start
```
Open a second terminal and run:
```
dfx deploy
```
After the deploy is finish, run:
```
npm start
```

PS: check the console to know in what port it's running...