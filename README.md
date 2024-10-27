# Vana-Node-Run-Full-Guide

## Claim Faucet (Moksha) [Use Only Burner Wallet or New Wallet]

🍀Go:- https://faucet.vana.org/moksha

### Moksha Testnet RPC

RPC URL - ``` https://rpc.moksha.vana.org ```

Chain ID - ``` 14800 ```

Network name - ``` Vana Moksha Testnet ```

Currency - ``` VANA ```

Block Explorer - ``` https://moksha.vanascan.io ```

## Web Miner

🍀Go:- https://sixgpt.xyz/

👉Click Sign Up/Login > Connect ur Burner Wallet OR New Wallet (u get faucet already)

👉Then Connect ur Google Account 

👉Then Click "START" button & Your Miner is start now (Must open ur browser in background -- More Uptime means More Reward)

### 🔶For Next Day Run This Command
Connect Wallet and Click on Start (Run Every Day when u Start ur PC)

## CLI Miner

### Need Some Requirements for PC Users

1. Install Docker - https://www.docker.com/products/docker-desktop/

2. Install WSL - https://learn.microsoft.com/en-us/windows/wsl/install#install-wsl-command

1️⃣ Take Faucet [Use Only Burner Wallet or New Wallet]

➡Claim Faucet - https://faucet.vana.org/moksha

🍀For VPS (Additional Only for VPS Users to Download Docker)
```
sudo apt update -y
```
```
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y
```
```
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
```
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
```
sudo apt update -y
```
```
apt-cache policy docker-ce
```
```
sudo apt install docker-ce -y
```
```
sudo usermod -aG docker ${USER}
su - ${USER}
groups
```

2️⃣ Check Docker Version
```
docker --version
```

3️⃣ Clone the repository
```
git clone git@github.com:sixgpt/miner.git
cd miner
```

4️⃣ Set the following environment variables
```
export VANA_PRIVATE_KEY=your_private_key
export VANA_NETWORK=moksha
```

5️⃣ Run the miner
```
docker compose up
```

## Notes
- You must have logged into sixgpt.xyz with your wallet before running the miner
- Make sure the wallet associated with your vana private key has enough $VANA balance on the desired network (at least 0.1)


## 🔶For Next Day Run This Command

#1 Open docker 1st 

#2 Now Open WSL and Put this Command 
```
cd miner
```
```
docker compose up
```

## Notes
- You must have logged into sixgpt.xyz with your wallet before running the miner
- Make sure the wallet associated with your vana private key has enough $VANA balance on the desired network (at least 0.1)
