# TELEGRAM PROXY SERVER

## HTTP SERVER

Instalar Squid Proxy

```bash
sudo apt update
sudo apt install squid
```

```bash
systemctl status squid.service
sudo nano /etc/squid/squid.conf
```

sudo apt install apache2-utils
sudo htpasswd -c /etc/squid/passwords <username>

My username, password and port are stored in bitwarden

sudo cat /etc/squid/passwords

sudo nano /etc/squid/squid.conf

```bash
#
# INSERT YOUR OWN RULE(S) HERE TO ALLOW ACCESS FROM YOUR CLIENTS
#
include /etc/squid/conf.d/*.conf
auth_param basic program /usr/lib/squid3/basic_ncsa_auth /etc/squid/passwords
auth_param basic realm proxy
acl authenticated proxy_auth REQUIRED
http_access allow authenticated

# For example, to allow access from your local networks, you may uncomment the
# following rule (and/or add rules that match your definition of "local"):
# http_access allow localnet
http_access allow localhost

# And finally deny all other access to this proxy
http_access deny all
```
sudo systemctl restart squid.service
sudo ufw allow 3128

## TO-DO

- Cambiar a MT-Proto Server
- Comparar rendimiento entre ambos

## LINKS

<https://www.digitalocean.com/community/tutorials/how-to-set-up-squid-proxy-on-ubuntu-20-04>
