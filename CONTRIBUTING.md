# Contributing to ARCADE

ARCADE was built by a fixed team during the Epitech curriculum. Issues and pull requests are welcome.

## Project layout

The core is in `src/` (main loop, library loader, error handling), the graphics libraries in `src/NCurses`, `src/SDL2` and `src/SFML`, and the games in `games/`. Every library and game is built as a shared object in `lib/`. See the [README](README.md) to build and run it.

## Workflow

1. Open an issue describing the bug or the change.
2. Create a branch from `main`: `<topic>` in one word, like the existing `graphics` or `switchLib` branches.
3. Commit with the convention of the history: `type(scope): summary`, e.g. `feat(core): instantiate run function`.
4. Open a pull request into `main` with a short list of the changes and `Closes #<issue>`.

## Code style

- C++ with `-Wall -Wextra`, no warnings.
- A new graphics library or game implements the interfaces of `include/`, see the [technical documentation](doc/arcade_documentation_implementation_lib.md).

## Code of conduct

By contributing you agree to follow the [code of conduct](CODE_OF_CONDUCT.md).
