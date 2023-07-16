# karentexas2
sudo apt update && sudo apt upgrade -y

apt install ufw -y 
ufw allow ssh 
ufw allow https 
ufw allow http 
ufw allow 30333
ufw allow 8078
ufw enable

sudo mkdir -p /etc/apt/keyrings
curl -fsSL repo.chainflip.io/keys/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/chainflip.gpg

gpg --show-keys /etc/apt/keyrings/chainflip.gpg
