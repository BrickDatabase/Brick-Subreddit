```yaml
milestone:
    iteration: 01
    title: "Brick-Subreddit"
    date: "April 30, 2021"
group:
    number: 3
    name: "Brick Database"
    members:
    - "Amina Mahmood"
    - "Aaron Joel Parker"
    - "Edward Riley"
```

# Brick-Subreddit

## Deployment and Packaging

### Deployment

#### Installation
##### Installing NodeJS
- **MacOS**: using [homebrew](https://brew.sh/) `brew install node`
- **Windows 10**: Install NodeJS from [NodeJS's website](https://nodejs.org/en/download/)
- **Linux**: Install NodeJS `sudo apt install node` & `sudo apt install npm`
##### Installing Python3
- **MacOS**: using [homebrew](https://brew.sh/) `brew install python`, it will install the latest which is Python3.
- **Windows 10**: download from [Python.org](https://www.python.org/downloads/)
- **Linux**: Install Python3 with advanced package tool `sudo apt install python3.8`
##### Cloning the Git Repository
- To clone a git address, go to the desired directory and type`git clone https://github.com/BrickDatabase/Brick-Subreddit.git`
- Once you cloned the git address, you need to navigate to cloned's directory and to update submodules to add each repos to the directory `git submodule update --init`

### Heroku's CLI and Deployment
#### Installation
- **MacOS**: Install heroku CLI using [homebrew](https://brew.sh/) `brew install heroku/brew/heroku`
- **Windows 10**: [Window 10's Installer](https://cli-assets.heroku.com/heroku-x64.exe)
- **Linux**: [List of Linux Supported](#Linux-Support) If you haven't install snap package yet then do this first `sudo apt install snapd` and then install heroku `sudo snap install heroku --classic`
- Navigate to service-layer and login using heroku account `heroku login`
- Add the sand-brickheroes's url `git remote add heroku https://git.heroku.com/sand-brickheroes.git`
- Navigate to application-layer and login again using heroku account `heroku login`
- Add the brickheroes's url `git remote add heroku https://git.heroku.com/brick-subreddit.git`
#### Commands
- To deploy the repo to heroku `git push heroku main`
- To turn on the website `heroku ps:scale web=1`
- To turn off the website `heroku ps:scale web=0`
- To open up the website `heroku open`
- Provision the database `heroku addons:create heroku-postgresql:hobby-dev`
- To check how much dynos is available `heroku ps`

### Pip3 Package

#### Installation
- Install package individually `pip3 install <MODULE_NAME>`
- Install all packages from requirements.txt `pip3 install -r requirements.txt`

#### Commands
- To run python file `Python3 filename.py`
- To test python file `PyTest filename.py`

### Npm Package

#### Installation
- Install package individually `npm install <package_name>`
- To install all packages from packages.json `npm i`

#### Commands
- To run NodeJS file `npm start`
- To Test NodeJS file `npm run mocha`



## Linux Support
Any Linux OS that are using **snap** or can be install with **snap** natively without needing to do workaround.
- Debian
- Ubuntu
- ElementaryOS
- POP!_OS
- ArchLinux