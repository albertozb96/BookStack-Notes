# SSH

## WINDOWS

- Parece que se instala automáticamente junto a Git.

## INVESTIGAR

- Cambiar path del .ssh (en Windows)

## COMMANDS

	ssh-keygen (falta el algoritmo??)
	ssh-keygen -t rsa -b 4096

## QUE NO SE CAIGA

https://unix.stackexchange.com/questions/34004/how-does-tcp-keepalive-work-in-ssh
https://askubuntu.com/questions/1343677/ssh-terminal-always-freezes-after-2minutes-of-inactivity
https://unix.stackexchange.com/questions/3026/what-do-options-serveraliveinterval-and-clientaliveinterval-in-sshd-config-d

investigar cuanto tiempo tarda en caerse para poner bien el archivo (tcpdump)
ponerlo en el host configs
