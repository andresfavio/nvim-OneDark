[![Screenshot-2023-12-19-22-54-25-1366x768.png](https://i.postimg.cc/zBwMk6sQ/Screenshot-2023-12-19-22-54-25-1366x768.png)](https://postimg.cc/xJCtfxTG)


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

## 🛠️ Instalacion de Neovim

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
  git clone https://github.com/andresfavio/nvim.git ~/.config/nvim
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

## 📂 Estructura de archivos

```bash
~/.config/nvim
├──init.lua
├──lua
│  ├──andres
│  │  ├──discipline.lua
│  │  └──utils.lua
│  ├──config
│  │  ├──autocmds.lua
│  │  ├──keymaps.lua
│  │  ├──lazy.lua
│  │  └──options.lua
│  ├──plugins
│  │  ├──coding.lua
│  │  ├──colorscheme.lua
│  │  ├──disable.lua
│  │  ├──editor.lua
│  │  └──ui.lua
│  └──util
│     └──debug.lua
└──README.md
```

### 🌈 Tema: 

Incluye el popular tema One Dark con varias variantes. Consulta el repositorio de Navarasu One Dark para obtener más detalles y opciones de configuración. [Repositorio de Navarasu One Dark](https://github.com/navarasu/onedark.nvim/blob/master/README.md)

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

[Lazy.nvim](https://github.com/folke/lazy.nvim) es un plugin para el editor de texto Neovim que proporciona funcionalidades de carga diferida (lazy loading) para mejorar el rendimiento y la velocidad de carga de los complementos y extensiones utilizados en Neovim. Con lazy.nvim, los complementos y extensiones se cargan solo cuando se necesitan, lo que ayuda a reducir el tiempo de inicio de Neovim y a mejorar la experiencia del usuario al trabajar con el editor.

[![Screenshot-2023-12-19-22-59-26-1366x768.png](https://i.postimg.cc/vHx7FfBY/Screenshot-2023-12-19-22-59-26-1366x768.png)](https://postimg.cc/CzYnbZkX)

Lazy.nvim utiliza una estrategia de carga diferida basada en eventos, lo que significa que los complementos y extensiones se cargan automáticamente cuando se realiza una acción específica que los requiere. Por ejemplo, si se utiliza una función o un comando proporcionado por un complemento, lazy.nvim se encargará de cargar ese complemento en ese momento para que esté disponible para su uso.

## Dashboard

El plugin [Dashboard.nvim](https://github.com/nvimdev/dashboard-nvim) es un complemento para Neovim que proporciona un panel de inicio personalizable y visualmente atractivo. El panel de inicio es la primera pantalla que se muestra al abrir Neovim y puede contener información útil, como archivos recientes, proyectos, notas, tareas pendientes y más.

[![Screenshot-2023-12-19-20-00-24-1366x768.png](https://i.postimg.cc/4dF8wG8B/Screenshot-2023-12-19-20-00-24-1366x768.png)](https://postimg.cc/34mCJsQv)

Con [Dashboard.nvim](https://github.com/nvimdev/dashboard-nvim), puedes personalizar el contenido y el diseño del panel de inicio según tus preferencias. Puedes agregar widgets, como listas de archivos, calendarios, relojes, citas inspiradoras y cualquier otra cosa que desees tener a mano al iniciar Neovim.

## Treesitter

[Treesitter](https://github.com/nvim-treesitter/nvim-treesitter) es un componente que se encuentra dentro de Neovim y permite al editor leer y analizar el código fuente de manera similar a un compilador. Escanea el código, recopila información sobre cada símbolo y genera un árbol de sintaxis, convirtiendo así el código en una estructura de datos que Neovim puede consultar

[![Screenshot-2023-12-19-23-07-57-1366x768.png](https://i.postimg.cc/s2MwnXLq/Screenshot-2023-12-19-23-07-57-1366x768.png)](https://postimg.cc/d7K23qwj)

El plugin [Treesitter](https://github.com/nvim-treesitter/nvim-treesitter) es una herramienta que utiliza Treesitter para agregar funcionalidades a Neovim. Proporciona varios módulos que se pueden utilizar para aprovechar las ventajas de Treesitter. Algunos de estos módulos incluyen resaltado de sintaxis mejorado, resaltado de paréntesis, resaltado de ámbito, resaltado de referencias y mucho más. 

## Lualine

El plugin [Lualine](https://github.com/nvim-lualine/lualine.nvim) es una barra de estado personalizable para Neovim. Proporciona información útil en la parte inferior de la ventana de Neovim, como el modo de edición, el nombre del archivo, el estado de Git, el número de línea actual y más.

### [![Screenshot-2023-12-19-23-04-41-1366x768.png](https://i.postimg.cc/nrJjQR7T/Screenshot-2023-12-19-23-04-41-1366x768.png)](https://postimg.cc/JDp4fQpB)

## Telescope

El plugin [Telescope](https://github.com/nvim-telescope/telescope.nvim) es una herramienta de búsqueda y exploración para Neovim. Proporciona una interfaz interactiva que te permite buscar y navegar por diferentes tipos de archivos, como archivos en tu proyecto, archivos en el sistema de archivos, registros de Git, resultados de búsqueda y más.

[![Screenshot-2023-12-19-23-00-50-1366x768.png](https://i.postimg.cc/26XWgSNL/Screenshot-2023-12-19-23-00-50-1366x768.png)](https://postimg.cc/LYLh1RXm)

[Telescope](https://github.com/nvim-telescope/telescope.nvim) utiliza una combinación de filtros y acciones para ayudarte a encontrar y manipular la información de manera eficiente. Puedes buscar archivos por nombre, contenido o extensión, y también puedes realizar búsquedas en texto completo en tu proyecto. Además, puedes utilizar acciones para abrir archivos, previsualizar contenido, realizar acciones en archivos seleccionados y más.

## Mason

<p float="left">
<img width="412" alt="Onedark - dark" src="https://i.postimg.cc/L52W0SLP/Screenshot-2023-12-19-23-09-17-1366x768.png">
<img width="412" alt="Onedark - darker" src="https://i.postimg.cc/Kv9WQdzK/Screenshot-2023-12-19-23-09-30-1366x768.png">
</div></p>
<p float="left">
<img width="412" alt="Onedark - cool" src="https://i.postimg.cc/YCZsBYQM/Screenshot-2023-12-19-23-09-42-1366x768.png">
<img width="412" alt="Onedark - deep" src="https://i.postimg.cc/KYTsGj5L/Screenshot-2023-12-19-23-09-49-1366x768.png">
</div></p>
<p float="left">
<img width="412" alt="Onedark - warm" src="https://i.postimg.cc/htkp5gqG/Screenshot-2023-12-19-23-09-55-1366x768.png">
<img width="412" alt="Onedark - warmer" src="https://i.postimg.cc/wx45rHXd/Screenshot-2023-12-19-23-10-00-1366x768.png">
</div></p>

[Mason](https://github.com/williamboman/mason.nvim) es un complemento de Neovim que le permite administrar fácilmente herramientas de edición externas, como servidores LSP, servidores DAP, linters y formateadores a través de una sola interfaz. Se ejecuta en todos los lugares donde se ejecuta Neovim (en Linux, macOS, Windows, etc.), con solo un pequeño conjunto de requisitos externos necesarios. Los paquetes se instalan en el directorio de datos de Neovim (:h standard-path) de forma predeterminada. Los ejecutables están vinculados a un único directorio bin/, que mason.nvim añadirá a la PATH de Neovim durante la configuración, lo que permite un acceso sin problemas desde los builtins de Neovim (shell, terminal, etc.), así como otros plugins de terceros.

## Nvim-cmp

El plugin [Nvim-cmp](https://github.com/hrsh7th/nvim-cmp) es un motor de autocompletado para Neovim. Proporciona una funcionalidad de autocompletado inteligente y personalizable mientras escribes en Neovim. nvim-cmp se integra con diferentes fuentes de completado, como LSP (Language Server Protocol), snippets y más.

[![Screenshot-2023-12-19-23-06-50-1366x768.png](https://i.postimg.cc/nrGyHrpT/Screenshot-2023-12-19-23-06-50-1366x768.png)](https://postimg.cc/q6gbwktC)

Algunas características y aspectos destacados de nvim-cmp son:

- Autocompletado inteligente: nvim-cmp ofrece sugerencias de autocompletado basadas en el contexto mientras escribes en Neovim.
- Integración con LSP: se puede utilizar con servidores LSP para obtener sugerencias de autocompletado basadas en el análisis del código.
- Soporte de snippets: nvim-cmp es compatible con snippets, lo que te permite insertar fragmentos de código predefinidos de manera rápida y sencilla.
- Personalización: puedes personalizar el comportamiento y la apariencia del autocompletado según tus preferencias.
- Integración con otros plugins: nvim-cmp se puede integrar con otros plugins de Neovim para ampliar su funcionalidad.

## Nvim-lsp

El Protocolo de Servidor de Lenguaje (LSP, por sus siglas en inglés) es un estándar de comunicación entre editores de código y servidores de lenguaje. Permite que los editores de código, como Neovim, se comuniquen con servidores específicos de lenguaje para proporcionar características avanzadas, como autocompletado, resaltado de sintaxis, navegación de código y más.

[![Screenshot-2023-12-19-23-10-58-1366x768.png](https://i.postimg.cc/GpjGx1LV/Screenshot-2023-12-19-23-10-58-1366x768.png)](https://postimg.cc/HJVrTR79)

## Inspiración

* [LazyVim](https://www.lazyvim.org/)

* [Crafzdog](https://www.youtube.com/watch?v=fFHlfbKVi30&pp=ygUJZGV2YXNsaWZl)
* [Josean-Dev](https://github.com/josean-dev/dev-environment-files)
* [Gentleman Programming](https://www.youtube.com/@GentlemanProgramming)

