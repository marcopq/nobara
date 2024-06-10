# nobara
Si ya hay una partición EFI de otro OS, se puede usar una partición btrfs y con calamares elegir la opción de reemplazar partición (se perderá el contenido de la partición btrfs), el instalador la usará automáticamente sin borrar la partición EFI sin afectar al otro OS y el dual boot.
## Paquetes
```
sudo dnf install shairport-sync btop ripgrep duperemove syncthing input-remapper tldr evtest trash-cli
```
```
flatpak install org.keepassxc.KeePassXC com.brave.Browser md.obsidian.Obsidian org.gnome.World.PikaBackup com.usebottles.bottles org.kde.haruna it.mijorus.gearlever
```
### Homebrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Seguir pasos instrucciones luego de la instalación (editar .bashrc).
```
brew install zsh zinit fzf oh-my-posh zoxide
```
## Servicios
```
systemctl --user enable --now syncthing.service
```
## Instalar fuentes
Desde una instalación de Windows copiar fuentes desde `Windows/Fonts` hacia:
```
mkdir ~/.local/share/fonts/Windows
```
Descomprimir Nerd Font y pegar en la misma carpeta:
```
curl -OL https://github.com/ryanoasis/nerd-fonts/releases/latest/download/JetBrainsMono.tar.xz
```
Ver si el sistema las reconoce con:
```
fc-list ':' file
```
# Post Instalación
- En Brave ir a `brave://flags/` habilitar Middle button autoscroll para hacer scroll más rápido.
