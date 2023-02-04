# Jupyter notebooks

## 1. Get started

### 1.1 Install anaconda
  
#### 1.1.1 MacOS

- Install anaconda
  - Option 1. Using [homebrew](https://brew.sh/index_sv): `brew install --cask anaconda`
    - Configure bash and/or zsh by running command in terminal
      - bash: `/usr/local/anaconda3/bin/conda init bash`
      - zsh: `/usr/local/anaconda3/bin/conda init zsh`
    - Close terminal
  - Option 2. Anaconda GUI installer <https://www.anaconda.com/products/distribution#macos>
- Update `conda update -n base -c defaults conda`

#### 1.1.2 WSL2

1. Download anaconda install script `wget https://repo.continuum.io/archive/Anaconda3-2022.10-Linux-x86_64.sh`
2. Run install script `sh Anaconda3-2022.10-Linux-x86_64.sh`
3. Add conda to bash and/or zsh `$HOME/anaconda3/bin/conda init bash` and `$HOME/anaconda3/bin/conda init zsh`
4. Update conda `conda update -n base -c defaults conda`

### 1.2 Config development environment

1. Create a virtual environment `conda create --name notebooks3.9 python=3.9 anaconda`
2. Activate notebook `conda activate notebooks3.9`
3. Install packages `conda install pandas pandas-datareader matplotlib ipython`
4. Install yfinance from conda-forge `conda install -c conda-forge yfinance`
5. Install the IPython kernel `ipython kernel install --user --name=notebooks3.9`

### 1.3. Visual Studio Code settings

- Install vscode extensions in `settings.json`
