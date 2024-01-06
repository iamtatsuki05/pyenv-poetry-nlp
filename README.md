# pyenv-poetry-nlp
Building an environment with pyenv+poetry on Mac

## How to setup
1. Start Terminal
2. Installing Homebrew`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
3. Installing Pyenv`brew install pyenv`
4. Path setting`export PYENV_ROOT="$HOME/.pyenv"`
5. `export PATH="$PYENV_ROOT/bin:$PATH"`
6. `eval "$(pyenv init --path)"`
7. `eval "$(pyenv init -)"`
8. Reload the Path configuration file`source ~/.bash_profile`
9. Check the version you want to install in pyenv`pyenv install --list`
10. Install version 3.9 this time.`pyenv install 3.10.11`
11. Change the version of the global`pyenv global 3.10.11`
12. Change local version`pyenv local 3.10.11`
13. Check to see if version changes have been applied`python --version`
14. Install Directory`git clone https://github.com/iamtatsuki05/pyenv-poetry.git`
15. Go to a directory with the command`cd <hogehoge>`
16. Installing packages with poetry`poetry install`
17. If you want to add libraries, etc. to poetry`poetry add librarie`

## Directory structure
```text
./
├── .git
├── .gitattributes
├── .github
├── .gitignore
├── .pre-commit-config.yaml
├── LICENSE
├── Makefile
├── README.md
├── compose.yaml
├── config
├── data
│   ├── datasets
│   ├── misc
│   ├── models
│   ├── outputs
│   └── raw
├── docs
├── env.sample
├── notebooks
├── poetry.lock
├── pyproject.toml
├── scripts
│   └── main.py
├── src
│   ├── __init__.py
│   └── project
│       ├── common
│       ├── config
│       ├── env.py
│       └── main.py
└── tests
    └── project
```
