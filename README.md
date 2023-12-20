[![Screenshot-2023-12-19-22-54-25-1366x768.png](https://i.postimg.cc/zBwMk6sQ/Screenshot-2023-12-19-22-54-25-1366x768.png)](https://postimg.cc/xJCtfxTG)

# Tabla de contenido

- [Descripción](#Descripcion)
- [Funciones](#funciones)
- [Requisitos](#requisitos)
  - [Ubuntu/Debian](#ubuntudebian)
  - [Fedora](#fedora)
  - [Arch Linux](#arch-linux)
  - [openSUSE](#opensuse)
  - [macOS (Homebrew)](#macos-homebrew)
- [Instalación de Nerd Fonts](#instalación-de-nerd-fonts)
- [Instalación](#instalación)
  - [Linux/MacOS](#linuxmacos)
- [Tema](#tema)
  - [One Dark](#one-dark)
- [Lazy](#lazy)
- [Dashboard](#dashboard)
- [Treesitter](#treesitter)
- [Lualine](#lualine)
  - [Captura de Pantalla Lualine](#captura-de-pantalla-lualine)
- [Telescope](#telescope)
- [Mason](#mason)
- [Capturas de Pantalla Mason](#capturas-de-pantalla-mason)
- [Nvim-cmp](#nvim-cmp)
- [Nvim-lsp](#nvim-lsp)

## 🚀 Descripción

El proyecto Neovim es un conjunto de configuraciones y complementos cuidadosamente seleccionados para mejorar la experiencia de usuario en Neovim. Diseñado pensando en la productividad y la personalización, este conjunto ofrece características avanzadas y atajos inteligentes para potenciar tu flujo de trabajo en el entorno de Neovim.

> **El proyecto usa como base las configuraciones del proyecto [LazyVim](https://github.com/LazyVim/LazyVim)** 

## ✨ Funciones 

- 🔥 Transforma tu Neovim 
- 🚀 Increíblemente rápido 
- 🧹 Configuración predeterminada sana para opciones, autocmds y mapas de teclas 
- 📦 Viene con una gran cantidad de complementos preconfigurados y listos para usar
- 💤 Personaliza y amplía fácilmente tu configuración con [lazy.nvim](https://github.com/folke/lazy.nvim) 

## ⚡️ Requisitos

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

## 🛠️ Instalacion de Requisitos:

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

## Instalación de Nerd Fonts:

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

## 🛠️ Instalacion

### Linux/MacOs

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

## Tema: 

#### One Dark:

Para poder configurar o conocer mejor el tema dirigete al repositorio de [navarazu one dark](https://github.com/navarasu/onedark.nvim/blob/master/README.md)

<p float="left">
<img width="412" alt="Onedark - dark" src="https://user-images.githubusercontent.com/20145075/144289835-cbbbcb22-4eae-41f1-a5a3-e1800a37ae41.png">
<img width="412" alt="Onedark - darker" src="https://user-images.githubusercontent.com/20145075/144293945-ee3b7dca-b119-4709-96d3-50391c7b8aba.png">
</div></p>
<p float="left">
<img width="412" alt="Onedark - cool" src="https://user-images.githubusercontent.com/20145075/144298826-5c51eb3a-5529-4fe7-bce2-56508eda93d7.png">
<img width="412" alt="Onedark - deep" src="https://user-images.githubusercontent.com/20145075/144299487-a7e886c7-2cc9-4d85-9aac-8517170432fc.png">
</div></p>
<p float="left">
<img width="412" alt="Onedark - warm" src="https://user-images.githubusercontent.com/20145075/144304677-abbf6cc1-4adc-48b4-b675-6f6a5a98b426.png">
<img width="412" alt="Onedark - warmer" src="https://user-images.githubusercontent.com/20145075/144304700-1e333a12-6994-4fb2-9053-1e7f294d41a6.png">
</div></p>

## Lazy

[![Screenshot-2023-12-19-22-59-26-1366x768.png](https://i.postimg.cc/vHx7FfBY/Screenshot-2023-12-19-22-59-26-1366x768.png)](https://postimg.cc/CzYnbZkX)

## Dashboard

[![Screenshot-2023-12-19-20-00-24-1366x768.png](https://i.postimg.cc/4dF8wG8B/Screenshot-2023-12-19-20-00-24-1366x768.png)](https://postimg.cc/34mCJsQv)

## Treesitter

[![Screenshot-2023-12-19-23-07-57-1366x768.png](https://i.postimg.cc/s2MwnXLq/Screenshot-2023-12-19-23-07-57-1366x768.png)](https://postimg.cc/d7K23qwj)

## Lualine

### [![Screenshot-2023-12-19-23-04-41-1366x768.png](https://i.postimg.cc/nrJjQR7T/Screenshot-2023-12-19-23-04-41-1366x768.png)](https://postimg.cc/JDp4fQpB)

## Telescope

[![Screenshot-2023-12-19-23-00-50-1366x768.png](https://i.postimg.cc/26XWgSNL/Screenshot-2023-12-19-23-00-50-1366x768.png)](https://postimg.cc/LYLh1RXm)

## Mason

[![Screenshot-2023-12-19-23-09-17-1366x768.png](https://i.postimg.cc/L52W0SLP/Screenshot-2023-12-19-23-09-17-1366x768.png)](https://postimg.cc/xJpgcWsj)

[![Screenshot-2023-12-19-23-09-30-1366x768.png](https://i.postimg.cc/Kv9WQdzK/Screenshot-2023-12-19-23-09-30-1366x768.png)](https://postimg.cc/crnTLkfZ)

[![Screenshot-2023-12-19-23-09-42-1366x768.png](https://i.postimg.cc/YCZsBYQM/Screenshot-2023-12-19-23-09-42-1366x768.png)](https://postimg.cc/YvN314Xs)

[![Screenshot-2023-12-19-23-09-49-1366x768.png](https://i.postimg.cc/KYTsGj5L/Screenshot-2023-12-19-23-09-49-1366x768.png)](https://postimg.cc/hJS0MS6P)

[![Screenshot-2023-12-19-23-09-55-1366x768.png](https://i.postimg.cc/htkp5gqG/Screenshot-2023-12-19-23-09-55-1366x768.png)](https://postimg.cc/dh92hb3M)

[![Screenshot-2023-12-19-23-10-00-1366x768.png](https://i.postimg.cc/wx45rHXd/Screenshot-2023-12-19-23-10-00-1366x768.png)](https://postimg.cc/5jvFHhKP)

## Nvim-cmp

[![Screenshot-2023-12-19-23-06-50-1366x768.png](https://i.postimg.cc/nrGyHrpT/Screenshot-2023-12-19-23-06-50-1366x768.png)](https://postimg.cc/q6gbwktC)

## Nvim-lsp

[![Screenshot-2023-12-19-23-10-58-1366x768.png](https://i.postimg.cc/GpjGx1LV/Screenshot-2023-12-19-23-10-58-1366x768.png)](https://postimg.cc/HJVrTR79)

