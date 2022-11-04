# Troglo Gamer Structure Library

### status

[![Linux Users](https://github.com/troglodyte-stdlib/troglo-player-c/actions/workflows/ci_runner_linux.yml/badge.svg)](https://github.com/troglodyte-stdlib/troglo-player-c/actions/workflows/ci_runner_linux.yml) [![MacOSX Users](https://github.com/troglodyte-stdlib/troglo-player-c/actions/workflows/ci_runner_macosx.yml/badge.svg)](https://github.com/troglodyte-stdlib/troglo-player-c/actions/workflows/ci_runner_macosx.yml) [![Windows Users](https://github.com/troglodyte-stdlib/troglo-player-c/actions/workflows/ci_runner_windows.yml/badge.svg)](https://github.com/troglodyte-stdlib/troglo-player-c/actions/workflows/ci_runner_windows.yml)

## overview

* * *

Gameplay is the specific way in which players interact with a game, and in
particular with video games. Gameplay is the pattern defined through the
game rules, connection between player and the game, challenges and overcoming
them, plot and player's connection with it. Video game gameplay is distinct
from graphics and audio elements. In card games, and the equivalent term is play.

A gamer is a proactive hobbyist who plays interactive games, especially video
games, tabletop role-playing games, and skill-based card games, and who plays
for usually long periods of time. The gamer structure is a gamer with actions
the gamer can make in a game depending on if the game is a command-line or
a video game.

## tooling

* * *

The targeted audience we are building for is *Windows 10*, *MacOSX*, *ChromeOS*
and *Linux* users. This project uses [Meson](https://mesonbuild.com/) `0.63.0`
and newer, uses `c2x` standards for initial implementation of the package. The
objective by far is usability, security, transparency, and lightweight, packages
for any if not most of your application development needs.

## Setup, Compile and Install

* * *

Using this package should be fairly simple just add the git wrap file
in your subprojects directory and include the dependency in your project.

```console
[wrap-git]
directory = troglo-struct-gamer-c
url = https://github.com/troglodyte-stdlib/troglo-struct-gamer-c.git
revision = main

[provide]
troglo-struct-gamer-c = trog_struct_gamer_dep
```


The next step should be to add the package to your Meson project:

```meson
trog_dep = dependency('troglo-struct-gamer-c')

executable('prog', 'main.c',
    dependencies : [trog_dep])

```

And finally we setup, and compile the project just like normal.

## usage

* * *

Here is a simple sample application that should get you up and
running with using this library as soon as possible but to learn
more please view the API documentation thanks.

**Usage in C**:

```c
//
// Troglobyte stdlib:
// author: Michael Gene Brockus
// gmail: <michaelbrockus@gmail.com>
//
#include <stdio.h>
#include <troglodyte/struct-gamer.h>


//
// main is where all good examples start
//
int main(void)
{
    printf("%s\n", greet());
    return 0;
} // end of func

```

## contact

If you want to contact me and have a few questions
regarding the solutions in the programming you can write
me a letter, my Gmail is <michaelbrockus@gmail.com>.

You may find that I have some social media platforms
in which you can follow me. [LinkedIn](https://www.linkedin.com/in/michael-brockus), [Facebook](https://facebook.com/michael.brockus.555), and [Instagram](https://instagram.com/troglodyte_coder/)
