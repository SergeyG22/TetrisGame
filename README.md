### Tetris

Classic Tetris - a computer game invented in the USSR.
Drop shapes and fill in as many horizontal lines as possible.


### Build from source
**MinGW compiler debug version:**

```
Select the compiler command line MinGW and go to the directory with the .pro file (example MinGW 7.3.0 64-bit command line)
Then enter the following commands:

mkdir build
cd build
qmake -makefile ..
mingw32-make debug

After entering the commands, an executable file will appear in the build folder.
```
**MinGW compiler release version:**

```
mkdir build
cd build
qmake -makefile ..
mingw32-make release
```
After entering the commands, an executable file will appear in the build folder.To add a DLL in the directory with Qt (not QtCreator, namely Qt of the desired version), there is a utility in the bin folder windeployqt.exe . Run it and it will copy the necessary files:
windeployqt.exe "the path to the application file." Choose it for your compiler (MinGW or MSVC).

---

**MSVC compiler debug version:**

```
Run vcvarsall.bat in directory vs19\VC\Auxiliary\Build
Select the compiler command line MSVC and go to the directory with the .pro file (example x64 Native Tools Command Promt)

Then enter the following commands:

mkdir build
cd build
qmake -makefile ..
nmake Debug

After entering the commands, an executable file will appear in the build folder.
```

**MSVC compiler release version:**

```
mkdir build
cd build
qmake -makefile ..
nmake Release
```
### Keyboard control

```
 W - move up
 S - move down
 A - move left
 D - move right
 SPACE - rotate figure
```

### Preview
![hippo](https://github.com/SergeyG22/TetrisGame/blob/master/docs/images/animation.gif)

