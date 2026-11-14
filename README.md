# ARCADE (v0.1)

![Arcade Game example picture](screenshots/arcade_game_picture.png)

### Development
By *Evans Ramin, Marin Jeunot & Sacha Lemée*.
```
evans.ramin@epitech.eu
```
```
marin.jeunot@epitech.eu
```
```
sacha.lemee@epitech.eu
```

### Contribution
Shared general architecture with *Nicolas Gonzales, Daniel Lozovan & Thibault Maillet*.
```
nicolas.gonzales@epitech.eu
```
```
daniel.lozovan@epitech.eu
```
```
thibault.maillet@epitech.eu
```

## Getting Started

### Prerequisites

- A C++ compiler (`g++` or `clang++`) and `make`
- ncurses, SDL2 + SDL2_ttf and **SFML 2.5/2.6** (SFML 3 is not supported)

```sh
# Ubuntu / Debian
sudo apt install build-essential pkg-config libncurses-dev libsdl2-dev libsdl2-ttf-dev libsfml-dev
# Fedora
sudo dnf install gcc-c++ make pkgconf ncurses-devel SDL2-devel SDL2_ttf-devel SFML-devel
```

### Build & Run

```sh
git clone git@github.com:sacha-lemee/arcade.git
cd arcade
make
./arcade ./lib/arcade_ncurses.so   # or ./lib/arcade_sdl2.so, ./lib/arcade_sfml.so
```

The games (Snake, Minesweeper) and the graphics libraries are built as shared libraries in `lib/` and can be switched at runtime:
`L` switch graphics library, `N` switch game, `R` restart, `Esc` back to menu, `E` quit.

### Documentation
- **[Technical Documentation](doc/arcade_documentation_implementation_lib.md)** (md file)
- **[Architecure Documentation](doc/arcade_uml_file.excalidraw)** (excalidraw file)
- dlopen/dlclose/dlsym: https://tldp.org/HOWTO/html_single/C%2B%2B-dlopen/?utm_source=chatgpt.com#externC

## License

This project is licensed under the **Creative Commons Attribution-ShareAlike 4.0 International License** (CC BY-SA 4.0 DEED).

![Arcade Project License](screenshots/License_AttributionShareAlike_4.0_International.png)
