# aws
# commands:

sudo apt update

sudo apt-get purge needrestart -y

sudo apt install python3-pip -y

sudo apt install nodejs -y

sudo apt install npm -y

sudo npm install pm2 -g

sudo apt install mysql-client -y


git clone https://github.com/HjayejMohamed/aws.git

python3 -m pip install -r aws/requirements.txt

cd aws

pm2 start echosystem.config.json



pm2 startup

sudo env PATH=$PATH:/usr/bin /usr/local/lib/node_modules/pm2/bin/pm2 startup systemd -u ubuntu --hp /home/ubuntu

pm2 save
