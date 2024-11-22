# VPS

## CONNECT TO VPS

```bash
ssh ubuntu@217.182.68.149
```

## CONFIGURAR SSH

Edit ssh config file

```bash
sudo nano /etc/ssh/sshd_config
```

uncomment to avoid lost connection:

```bash
TCPKeepAlive yes
ClientAliveInterval 60
ClientAliveCountMax 3
```

After that save and reboot

```bash
sudo reboot
```

## SSH CON GIT EN SERVER

- Generar la ssh-keygen
- cat /home/ubuntu/.ssh/id_rsa.pub
- copiar y pegar en github
