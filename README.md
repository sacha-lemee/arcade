# ARCADE

![ARCADE Game example picture](screenshots/arcade_game_picture.png)

### Development

By *Evans Ramin*(evans.ramin@epitech.eu), *Marin Jeunot*(marin.jeunot@epitech.eu) & *Sacha Lemée*(sacha.lemee@epitech.eu).

Shared general architecture with *Nicolas Gonzalez*(nicolas.gonzalez@epitech.eu), *Daniel Lozovan*(daniel.lozovan@epitech.eu) & *Thibault Miallet*(thibault.miallet@epitech.eu), so that the graphics libraries and games of both groups are interchangeable.

## Objective

A gaming platform that loads its graphics libraries and its games at runtime, as shared libraries, and lets the player switch between them without restarting.

## Features

- Graphics libraries: **ncurses**, **SDL2** and **SFML**, each built as a shared library in `lib/`
- Games: **Snake** and **Minesweeper**
- A menu listing the available libraries and games, with player scores
- Switch library or game at any time while playing

## Getting Started

### Prerequisites

This project requires:
- A C++ compiler (`g++` or `clang++`) and `make`
- ncurses, SDL2 + SDL2_ttf and **SFML 2.5/2.6** (SFML 3 is not supported)

```sh
# Ubuntu / Debian
sudo apt install build-essential pkg-config libncurses-dev libsdl2-dev libsdl2-ttf-dev libsfml-dev
# Fedora
sudo dnf install gcc-c++ make pkgconf ncurses-devel SDL2-devel SDL2_ttf-devel SFML-devel
```

### Installation for Linux

1. **Clone the repository:**

```sh
git clone git@github.com:sacha-lemee/arcade.git
cd arcade
```

2. **Build the project:**

```sh
make
```

3. **Run it with a starting graphics library:**

```sh
./arcade ./lib/arcade_ncurses.so   # or ./lib/arcade_sdl2.so, ./lib/arcade_sfml.so
```

| Key | Action |
|---|---|
| `L` | switch graphics library |
| `N` | switch game |
| `R` | restart the game |
| `Esc` | back to the menu |
| `E` | quit |

## Documentation

- [Technical documentation](doc/arcade_documentation_implementation_lib.md): how to add a graphics library or a game
- [Architecture diagram](doc/arcade_uml_file.excalidraw) (Excalidraw file)
- [C++ dlopen mini HOWTO](https://tldp.org/HOWTO/html_single/C++-dlopen/#externC)

## Contributing

Contributions are welcome: read [CONTRIBUTING.md](CONTRIBUTING.md) and the [code of conduct](CODE_OF_CONDUCT.md).

## License

This project is licensed under the **Creative Commons Attribution-ShareAlike 4.0 International License** (CC BY-SA 4.0), see [LICENSE](LICENSE).

![ARCADE License : CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-blue.svg)
