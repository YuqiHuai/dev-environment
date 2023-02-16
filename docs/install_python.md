# How to install Python on Ubuntu?

## Installing Python
1. `sudo add-apt-repository ppa:deadsnakes/ppa`
2. `sudo apt update`
3. `sudo apt install python3.11`

## Updating alternative
- `sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.11 1`
- `sudo update-alternatives --config python`
- `sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.11 1`
- `sudo update-alternatives --config python3`

## Installing without SUDO
1. `wget https://www.python.org/ftp/python/3.11.2/Python-3.11.2.tar.xz`
2. `tar -xf Python-3.11.2.tar.xz`
3. `cd Python-3.11.2`
4. `mkdir ~/.localpython`
5. `./configure --prefix=/home/$USER/.localpython`
6. `make`
7. `make install`
8. `echo "export PATH=\"/home/$USER/.localpython/bin:\$PATH\""`
9. `ln -s /home/$USER/.localpython/bin/python3 /home/$USER/.localpython/bin/python` >> ~/.bashrc

## Installing Poetry (Python package manager)
1. `curl -sSL https://install.python-poetry.org | python3 -`
