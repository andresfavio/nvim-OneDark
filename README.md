# Mi Configuracion De Neovim

# 🚀 Descripción

El proyecto Neovimes un conjunto de configuraciones y complementos cuidadosamente seleccionados para mejorar la experiencia de usuario en Neovim. Diseñado pensando en la productividad y la personalización, este conjunto ofrece características avanzadas y atajos inteligentes para potenciar tu flujo de trabajo en el entorno de Neovim.

> **El proyecto usa como base las configuraciones del proyecto [LazyVim](https://github.com/LazyVim/LazyVim)** 

# ✨ Funciones 

- 🔥 Transforma tu Neovim 
- 🚀 Increíblemente rápido 
- 🧹 Configuración predeterminada sana para opciones, autocmds y mapas de teclas 
- 📦 Viene con una gran cantidad de complementos preconfigurados y listos para usar
- 💤 Personaliza y amplía fácilmente tu configuración con [lazy.nvim](https://github.com/folke/lazy.nvim) 

# ⚡️ Requisitos

* Neovim \>= **0.9.0** 
* Git >= **2.19.0** 
* Fuente [Nerd Font](https://www.nerdfonts.com/) (v3.0 o superior) ***(opcional, pero necesaria para mostrar algunos iconos)***
* [lazygit](https://github.com/jesseduffield/lazygit) ***(optional)***
* Para el plugin telescope.nvim ***(opcional)***
  - **live grep**: [ripgrep](https://github.com/BurntSushi/ripgrep)
  - **find files**: [fd](https://github.com/sharkdp/fd)

* Un terminal que admita color verdadero y undercurl:
  * [kitty](https://github.com/kovidgoyal/kitty) ***(Linux & Macos)***
  * [wezterm](https://github.com/wez/wezterm) ***(Linux, Macos & Windows)***
  * [alacritty](https://github.com/alacritty/alacritty) ***(Linux, Macos & Windows)***
  * [iterm2](https://iterm2.com/) ***(Macos)***

# 🛠️ Instalacion de Requisitos:

### Ubuntu/Debian:

```bash
sudo apt-get update
sudo apt-get install neovim
sudo apt-get install git
sudo apt-get install lazygit 
sudo apt-get install ripgrep 
sudo apt-get install fd-find 
sudo apt-get install fzf
```

### Fedora:

```bash
sudo dnf install neovim
sudo dng install git
sudo dnf install lazygit 
sudo dnf install ripgrep 
sudo dnf install fd-find 
sudo dnf install fzf
```

### Arch Linux:

```bash
sudo pacman -S neovim
sudo pacman -S git
sudo pacman -S lazygit 
sudo pacman -S ripgrep 
sudo pacman -S fd 
sudo pacman -S fzf
```

sino tambien puede usar yay:

### Yay

```bash
yay -S neovim
yay -S git
yay -S lazygit
yay -S ripgrep
yay -S fd
yay -S fzf
```

en caso de que no tengas yay:

Copia el repositorio:

```bash
cd
git clone https://aur.archlinux.org/yay.git
```

Entra en la carpeta de yay:

```bash
cd yay
```

Instala yay:

```bash
makepkg -si
```

Ahora si Instala los requerimientos con el comando:

```bash
yay -S (Nombre Del programa o dependencia que necesitas)
```

### openSUSE:

```bash
sudo zypper install neovim
sudo zypper install git
sudo zypper install lazygit 
sudo zypper install ripgrep
sudo zypper install fd
sudo zypper install fzf
```

### macOS (usando Homebrew):

```bash
brew install neovim
brew install git
brew install lazygit 
brew install ripgrep 
brew install fd
brew installfzf
```

Si aún no tienes Homebrew instalado, puedes instalarlo con:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Luego, puedes instalar los requerimientos o dependencias:

```bash
brew install (nombre del programa o dependencia que deseas instalar)
```

### Instalación de Nerd Fonts:

1. Clona el repositorio de Nerd Fonts desde GitHub:

```bash
git clone --depth 1 https://github.com/ryanoasis/nerd-fonts.git
```

2. Cambia al directorio del repositorio:

```bash
cd nerd-fonts
```

3. Ejecuta el script de instalación:

```bash
./install.sh
```

# 🛠️ Instalacion

## Linux/MacOs

Instalar el [LazyVim Starter](https://github.com/LazyVim/starter)

* Haz una copia de seguridad de tus archivos actuales de Neovim:

  ```bash
  mv ~/.config/nvim{,.bak}
  
  # Opcional pero recomendado
  mv ~/.local/share/nvim{,.bak}
  mv ~/.local/state/nvim{,.bak}
  mv ~/.cache/nvim{,.bak}
  ```

* Caso contrario que quieras eliminar los archivos para hacer una instalacion limpia:

  ```bash
  rm -rf ~/.config/nvim{,.bak}
  
  # Opcional pero recomendado
  rm -rf ~/.local/share/nvim{,.bak}
  rm -rf ~/.local/state/nvim{,.bak}
  rm -rf ~/.cache/nvim{,.bak}
  ```

* Clona el repositorio

  ```bash
  https://github.com/andresfavio/nvim.git
  ```

* Elimine la carpeta.git para poder agregarla a su propio repositorio más adelante

  ```bash
  rm -rf .git
  ```

* Inicia Neovim

  ```bash
  nvim
  ```

  Consulte la documentacion de [LazyVim](https://github.com/LazyVim/LazyVim) para poder personalizarlo a su gusto

  > Se recomienda ejecutar :checkhealth después de la instalación, esto para poder verificar si necesita instalar alguna dependencia extra.

  .......................