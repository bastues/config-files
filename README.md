# config-files
**ZSHRC** | Esta archivo a sido un fork de arhivo de *s4vitar* (enlace abajo) con ciertas modificaciones para ajuatarlo a nuestro gusto
https://s4vitar.github.io/bspwm-configuration-files/  
```
sudo apt install zsh
```
```
sudo usermod --shell /usr/bin/zsh proyecto
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

**POWERSHELL 10K** | Estos archivos son un fork del los archivos de configuracion de que se muestran en el video del creador *s4vitar* (enlace en la descripcion) con ciertas modificaciones para ajuatarlo a nuestro gusto 
https://www.youtube.com/watch?v=fshLf6u8B-w&t=3581s (minuto: 1:17:57)
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```
```
rm .p10.zsh
https://raw.githubusercontent.com/bastues/config-files/main/p10k/user/.p10k.zsh
```
(root)
```
usermod –shell /usr/bin/zsh root
ln -s -f /home/jorge/.zshrc /root/.zshrc
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
cd
rm .p10k.zsh
wget https://raw.githubusercontent.com/bastues/config-files/main/p10k/root/.p10k.zsh
```
