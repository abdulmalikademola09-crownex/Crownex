# Update System and Install Dependencies
sudo apt update && sudo apt upgrade -y
sudo apt install git ffmpeg curl -y

# Install Node.js (Version 20.x Recommended)
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt install nodejs -y

# Install Yarn and PM2 for Process Management
sudo npm install -g yarn
yarn global add pm2

# Clone the Repository and Install Dependencies
git clone https://github.com/M3264/Kord-Ai
cd Kord-Ai
npm install
