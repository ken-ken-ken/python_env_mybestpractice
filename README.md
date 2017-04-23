
My best practice building python environment in ubuntu env.

**WARNING: This is MY best practice. (Almost memo for myself)**

step 1, install pyenv (included in pyenv.sh)
dependencies
```
sudo apt-get install git gcc make openssl libssl-dev libbz2-dev libreadline-dev libsqlite3-dev
```

pyenv
```
git clone git://github.com/yyuu/pyenv.git ~/.pyenv
```

path (eg, in bashrc)
```
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
```

```
source ~/.bashrc
```

step 2, (optional: conda env)
miniconda (check available versions with pyenv install --list, and install)
```
pyenv global {name of anaconda or miniconda}
conda create -n {name of env} python=3.5
source ~/.pyenv/versions/{name of anaconda or miniconda}/bin/activate {name of env}
```