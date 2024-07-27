# 🃏 c solitaire
  
![Gameplay Demo](repo/recording.gif)

a small solitaire game programmed in C using [raylib](https://www.raylib.com/)  
play it online at [zaccnz.github.io/solitaire](https://zaccnz.github.io/solitaire/)  

## technologies
- [raylib](https://github.com/raysan5/raylib)  
- [raylib-nuklear](https://github.com/RobLoach/raylib-nuklear)  
- [PhysFS](https://icculus.org/physfs/)
- [tomlc99](https://github.com/cktan/tomlc99)  
- [CMake](https://cmake.org/)  

## features
- animated movement
- texture pack system
- timer and score
- leaderboard
- undo and redo
- web assembly build

## resources
- [2D Poker Pack](https://screamingbrainstudios.itch.io/poker-pack) - Screaming Brain Studios  
- [8Bit Deck Card Assets](https://drawsgood.itch.io/8bit-deck-card-assets) - DrawsGood
- [Card Asset Pack](https://natomarcacini.itch.io/card-asset-pack) - natomarcacini
- [Fantasy Card Game SFX Pack](https://olexmazur.itch.io/fantasy-card-game) - Olex Mazur  
- [Roboto](https://fonts.google.com/specimen/Roboto) - Google Fonts  
- WebKit WebCore's [UnitBezier.h](https://github.com/WebKit/WebKit/blob/main/Source/WebCore/platform/graphics/UnitBezier.h)  
- Solitaire Scoring from [lkcl](https://hands.com/~lkcl/hp6915/Dump/Files/soltr.htm)

## build instructions

this project uses CMake.  to get started:  
```
git clone https://github.com/danadrianmirea/solitaire --recurse-submodules
cd solitaire
mkdir build && cd build
cmake ..
```

to compile for the web (using EMSCRIPTEN, after running emsdk_env script)
```
git clone https://github.com/zaccnz/solitaire --recurse-submodules
cd solitaire
emcmake cmake -S . -B build -DPLATFORM=Web
cmake --build build
```
