# Instalação do Debian Sid

## Checklist

- - -


- [ ] Habilitar senha root

```
sudo passwd root
```

- - -

- [ ] Editar sources.list

```
sudo nano /etc/apt/sources.list
```

- - -

- [ ] Substituir repositórios por...

```
deb http://ftp.br.debian.org/debian/ sid main contrib non-free
deb-src http://ftp.br.debian.org/debian/ sid main contrib non-free
```

- - -

- [ ] Atualizar...

```
sudo apt update
```

- - -

- [ ] Baixar script de instalação dos programas iniciais

```
git clone https://github.com/debxp/sid-install.git
```

- - -

- [ ] Instalar aplicativos e complementos externos

### Diversos

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

- [ ] configurar o autostart do OpenBox

```
~/.screenlayout/default.sh &
xfce4-panel &
nitrogen --restore &
compton -cCGfFz -o 0.38 -O 200 -I 200 -t -15 -l -15 -r 10 -D 2 --shadow-exclude "class_g = 'Firefox' && argb" -b --backend glx --vsync opengl-swc &
/usr/lib/policykit-1-gnome/polkit-gnome-authentication-agent-1 &
xfce4-power-manager &
numlockx &
```
