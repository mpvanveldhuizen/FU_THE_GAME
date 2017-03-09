Fuck You The Game
===========
The title pretty much explains everything. This project was started as a learning experience, to learn game making as well was using the SDL libraries. It also was used to show how complete randomness in video games can be a terrible idea.

SDL needs to be installed in order to work.

For Windows, MinGW was used to compile.
Credit goes to [Lazy Foo Productions](http://lazyfoo.net/) for providing tutorials and instructions on how to set up SDL for multiple platforms.

Installing SDL
===========
## On Linux
```
apt-get install libsdl2-dev libsdl2-image-dev libsdl2-mixer-dev libsdl2-ttf-dev
```
or
```
yum install SDL2-devel SDL2_mixer-devel SDL2_image-devel SDL2_ttf-devel
```

## On Mac
Install [Homebrew](http://brew.sh/) paste the following in the terminal
```
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```  
Then install SDL with
```
brew install sdl2
```
## On Windows
We used MinGW to compile for windows. First is to install MinGW if you havent already. Follow this [guide](http://www.mingw.org/wiki/Getting_Started) to help install MinGW, and make sure gcc is installed.

1. Download the SDL Development Libraries
  * https://www.libsdl.org/release/SDL2-devel-2.0.5-mingw.tar.gz 
2. Open gz archive and there should be a *.tar archive inside.
3. Open the *.tar and there should be a folder inside of that.
4. Open the folder and it'll contain a bunch of subfolders.
5. Copy the contents of the lib subfolder to the MinGW lib folder.
  * The MinGW lib folder should be at `C:\MinGW\lib`.
6. After that, open the include subfolder in the archive and extract the folder named `SDL` to the MinGW include folder
  * Should be at `C:\MinGW\include`.
7. Now take the `SDL.dll` from the archive (it should be inside the bin subfolder) and extract it. You're going to put this in the same directory as your exe when you compile it.
8. Download the SDL extra libraries
  * https://www.libsdl.org/projects/SDL_image/release/SDL2_image-devel-2.0.1-VC.zip 
  * http://www.libsdl.org/projects/SDL_mixer/release/SDL2_mixer-devel-2.0.1-VC.zip
  * http://www.libsdl.org/projects/SDL_ttf/release/SDL_ttf-devel-2.0.1-VC.zip
9. Open up the zip archive and there should be a folder inside.
10. Open the folder and it'll contain 2 subfolders.
11. First, open the `include` subfolder in the archive and extract the header file inside to the SDL subfolder inside of the MinGW include folder. 
  * It should be at `C:\MinGW\include\SDL`.
12. Now find the `lib` folder from the archive. Take the library file(s) from the archive and put them with the rest of the SDL library files.
  * The MinGW lib folder should be at `C:\MinGW\lib`.
13. Now extract all of the `*.dll` file(s) from the `x86` folder in the archive and put them in the same directory as your exe.
