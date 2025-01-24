# Initia Weave CLI 

![image](https://github.com/user-attachments/assets/a077805e-88ef-42c6-a3e5-d08776586548)

#### Run the following command to update and upgrade system packages:

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Install Packages:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen unzip lz4 texlive-binaries -y
```

## Install GO :

```bash
cd $HOME
VER="1.23.0"
wget "https://golang.org/dl/go$VER.linux-amd64.tar.gz"
sudo rm -rf /usr/local/go
sudo tar -C /usr/local -xzf "go$VER.linux-amd64.tar.gz"
rm "go$VER.linux-amd64.tar.gz"
[ ! -f ~/.bash_profile ] && touch ~/.bash_profile
echo "export PATH=$PATH:/usr/local/go/bin:~/go/bin" >> ~/.bash_profile
source $HOME/.bash_profile
[ ! -d ~/go/bin ] && mkdir -p ~/go/bin
```

## Install CLI : 

```bash
git clone https://github.com/initia-labs/weave.git
cd weave
git checkout tags/v0.1.1
make install
```

## Create Gas Station Wallet : 
```bash
weave gas-station setup
```
![image](https://github.com/user-attachments/assets/86581ff0-50b3-4807-9332-dff29e96d50d)

- Save Your Mnemonic and Write Contine - Enter.

![image](https://github.com/user-attachments/assets/b23d1826-ea74-4c7a-b8ca-158549817536)


## Example : 

![image](https://github.com/user-attachments/assets/c0f35189-5ce4-45a1-992b-470ede9f7388)


## Faucet : 

INIT Test Faucet: [Initia Faucet](https://faucet.testnet.initia.xyz/)
TIA Test Faucet : [Celestia Faucet](https://docs.celestia.org/how-to-guides/mocha-testnet#mocha-testnet-faucet)
