# config-files
**ZSHRC** | Esta archivo a sido un fork de arhivo de *s4vitar* (enlace abajo) con ciertas modificaciones para ajuatarlo a nuestro gusto
https://s4vitar.github.io/bspwm-configuration-files/  
```
sudo apt install zsh
```
```
sudo usermod --shell /usr/bin/zsh <nombre usuario>
```
```
rm .zshrc
wget https://raw.githubusercontent.com/bastues/config-files/main/.zshrc
```
```
sudo apt install zsh-syntax-highlighting zsh-autosuggestions
```
```
cd /usr/share
sudo mkdir zsh-sudo
sudo chown usuario:grupo zsh-sudo
cd zsh-sudo
sudo wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/plugins/sudo/sudo.plugin.zsh
```

**KITTY** | Estos archivo es un fork del archivos de *rxyhn* (enalace abajo) con ciertas modificaciones para ajuatarlo a nuestro gusto 
https://github.com/rxyhn/tokyo/tree/main/config/kitty
```
sudo apt install kitty
```
```
sudo update-alternatives --config x-terminal-emulator
```
```
cd .config/kitty
wget https://raw.githubusercontent.com/bastues/config-files/main/kitty/color.ini
wget https://raw.githubusercontent.com/bastues/config-files/main/kitty/kitty.conf
```
```
Default Aplications > Utilities > kitty
```

**POWERSHELL 10K** | Estos archivos son un fork del los archivos de configuracion de que se muestran en el video del creador *s4vitar* (enlace en la descripcion) con ciertas modificaciones para ajuatarlo a nuestro gusto 
https://www.youtube.com/watch?v=fshLf6u8B-w&t=3581s (minuto: 1:17:57)
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```
```
rm .p10k.zsh
wget https://raw.githubusercontent.com/bastues/config-files/main/p10k/user/.p10k.zsh
```
(root) **cambia el nombre de usuario en el link simbolico**
[!CAUTION]
Asegurate en el link simbolico el modifcar el nombre del usuario.
```
usermod –shell /usr/bin/zsh root
ln -s -f /home/usuario/.zshrc /root/.zshrc
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
cd
rm .p10k.zsh
wget https://raw.githubusercontent.com/bastues/config-files/main/p10k/root/.p10k.zsh
```
**GPG** | Configuracion del gpg para que la cache no alamacene la contraseña en cache
```
cd .gnupg
nano gpg-agent.conf
wget https://raw.githubusercontent.com/bastues/config-files/main/gpg-agent.conf
gpgconf --kill gpg-agent
gpgconf --launch gpg-agent
```
**Fonts** Instalar fuente custom de [nerd fonts](https://www.nerdfonts.com/font-downloads)
```diff
cd /usr/share/fonts
sudo mkdir Customfont
cd Customfont
wget https://www.nerdfonts.com/font-downloads
-unzip "fuente.zip"
```


