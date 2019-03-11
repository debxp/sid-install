# Instalação do Debian Sid

## Checklist

- - -


- [ ] __Habilitar senha root__

```
sudo passwd root
```

- - -

- [ ] __Editar sources.list__

```
sudo nano /etc/apt/sources.list
```

- - -

- [ ] __substituir repositórios por...__

```
deb http://ftp.br.debian.org/debian/ sid main contrib non-free
deb-src http://ftp.br.debian.org/debian/ sid main contrib non-free
```

- - -

- [ ] __Atualizar...__

```
sudo apt update
sudo apt upgrade
```

- - -

- [ ] __Baixar script de instalação dos programas iniciais__

```
git clone https://github.com/debxp/sid-install.git
```

- - -

- [ ] __Instalar aplicativos e complementos externos__


* atom
* etcher
* filezila-theme-papirus
* github Desktop
* ibm-aspera-connect
* indicator-keylock
* nextcloud
* poddr
* simplenote
* whatsie
* xampp-linux
* yakyak

- - -

- [ ] __configurar o autostart do OpenBox__

```
~/.screenlayout/default.sh &
xfce4-panel &
nitrogen --restore &
compton -cCGfFz -o 0.38 -O 200 -I 200 -t -15 -l -15 -r 10 -D 2 --shadow-exclude "class_g = 'Firefox' && argb" -b --backend glx --vsync opengl-swc &
/usr/lib/policykit-1-gnome/polkit-gnome-authentication-agent-1 &
xfce4-power-manager &
numlockx &
```
