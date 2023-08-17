maze_projt
SDL2 and SDL2_image are required to compile and use this program
Compile with the following flags: gcc -O2 -g -Wall -Werror -Wextra -pedantic -I code/header code/*.c -lSDL2 -lSDL2_image -lm -o maze `sdl2-config --cflags --libs` 
Run the file : ./maze no_tex or ./maze maps/<map_name> no_tex

controls
Uu key : move forward
Down key : move backward
Left key : strafe left
Right key : strafe right
Q : rotate camera left
D : rotate camera right
F : toggle fullscreen
ESC : quit
Maps
The maps are defined in 2D arrays in text files, which are parsed when passed as an argument to the maze executable. 0 represents open space, all other integers are drawn as walls.
