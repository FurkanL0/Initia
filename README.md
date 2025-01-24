# Initia Weave CLI 

![image](https://github.com/user-attachments/assets/a077805e-88ef-42c6-a3e5-d08776586548)

#### Run the following command to update and upgrade system packages:

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Install Packages:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen unzip lz4 -y
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


- Claim Faucet And Check Youer Wallets : 
```bash
weave gas-station show
```
![image](https://github.com/user-attachments/assets/bb355332-5245-4ff3-9055-fd74294935ad)


## Start : 
```bash
weave init
```
![image](https://github.com/user-attachments/assets/559f9e01-e2a4-4f72-a477-86de3b97d67c)

## Run L1 Node : 

![image](https://github.com/user-attachments/assets/9ac4f784-b677-4451-a966-d137fa353320)

- Enter

#### Write Your Moniker : 

![image](https://github.com/user-attachments/assets/a3885ac7-0453-4245-a607-e4ea95dc67d4)

#### Chouse Your Options 

Space : Select - Enter : Sumbit

![image](https://github.com/user-attachments/assets/5018fa6c-79c1-48a7-840f-040b788f57b4)

#### Seeds : 

- If you want Specify seed paste your seed - i want initia offical seed press TAB and enter.


![image](https://github.com/user-attachments/assets/5e4d6560-a21a-479b-b311-d6417b0395c9)


- Tab for Polkachu and enter.

![image](https://github.com/user-attachments/assets/683b6891-0734-4880-ab58-5015f5f51fe0)

#### Pruning  : 

- Default.

![image](https://github.com/user-attachments/assets/c7b15127-72d1-4577-a232-7039a1a4a1b6)

#### Automatic Upgrade : 

- Yes - Enter.

![image](https://github.com/user-attachments/assets/ec222451-0be3-4d46-a5fa-62927b81f08a)


#### Snapshot : 

- I chose state sync. you can install snapshot if you want.

![image](https://github.com/user-attachments/assets/57c664d1-d8a7-439d-8835-350d7946a9f6)

- Tab for Polkachu State SYNC :

![image](https://github.com/user-attachments/assets/be70335a-8ad6-4ba8-9b50-861d7786ec6a)

#### Additional Peers : 

- Tab for Polkachu Peers. Enter.


![image](https://github.com/user-attachments/assets/7f789402-9e2f-4cb4-95de-97ebc4107bbf)

## Succsess : 

![image](https://github.com/user-attachments/assets/e3fbcca1-89ad-47f6-9b9b-c026949a0167)

## Start : 

- Screen : 

```bash
screen -S initia
```
- Start : 

```bash
weave initia start
```



