# EZ-DNS-Setter

I needed a quick way to set Iranian DNS servers like Shecan and 403 for my own use, so I wrote this simple script. Just provide the DNS name and connection name, and you're all set!

Since it was useful to me, I decided to share it.

Have a new DNS to add? Make a PR ✨

# Install
```shell
  git clone https://github.com/pooya-hajjar/ez-DNS-setter/edit/master/dns-setter ez-dns-setter
  sudo cp ./ez-dns-setter/dns-setter /usr/local/bin/
  sudo rm -rf ./ez-dns-setter
  sudo chmod +x /usr/local/bin/dns-setter
```

# Usage 
Now you can run the dns-setter script from anywhere on your system:

```shell
dns-setter <alias> <driver_name>
```
___
### Current list of aliases for DNS servers:
* none (to reset DNS to system automatic)
* cloudflare
* google
* shecan
* 403
* radar
* electro


___
### Finding your connection name:
Run this command to list your network connections:
```shell
nmcli connection show
```
Pick the connection NAME you want from the list.

