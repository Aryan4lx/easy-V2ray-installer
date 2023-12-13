# Install

```
bash <(curl -Ls https://raw.githubusercontent.com/Aryan4lx/easy-V2ray-installer/main/v2ray.sh)
```

if you are installing v2ray from scratch
you can use these steps (recomended):

1. Set domains
2. Install Nginx and get certs
3. Install 3X-UI panel
4. From x-ui install Geo, BBR, fail2ban(if you want, up to you)
5. Allow Ports you need using ufw
6. You can use the the ssl you got for your domain in your panel, for that you can use the command below to find the path

```
sudo certbot certificates
```

7. Install Warp (more details below)
8. Done

# Warp

for Warp you have the options to choose 3x-ui script from the panel itself
or you can use the one provided here made by hamid-gh98
if you use hamid-gh98 from my script add the json code below to your v2ray panel
https://yourdomain:port/panel/settings --> Xray Configuration --> Advanced Template

```
{
        "type": "field",
        "outboundTag": "WARP",
        "domain": [
          "regexp:.*"
        ],
        "ip": [
          "0.0.0.0/0"
        ]
      }
```

after the installation you can use the option

```
warp a
```

to change to warp plus (you can easily get warp plus key from telegram Bots or any other way possible on the internet)

# contact me in telegram https://t.me/ARS4lx
