# Readme

> In this repository I share the configurations made on my Debian 11 desktop. Currently used on my laptop.

# Instalar Google Chrome

cat << EOF > /etc/apt/sources.list.d/google-chrome.list
deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main
EOF

wget -O- https://dl.google.com/linux/linux_signing_key.pub |gpg --dearmor > /etc/apt/trusted.gpg.d/google.gpg

apt update

apt -y install google-chrome-stable
