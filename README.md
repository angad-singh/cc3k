# ChamberCrawler3000

Group project for second year CS course (CS246) at the University of Waterloo. This repo is not  actively maintained. Group members included Angad Singh, Lizhong Bi and Tianli Zhan. 

## Compilation and Execution 
To compile the game please execute `make` in the terminal. This will generate object files and compile all the necessary files.  Use `make clean` to clean up the object files. `make` executes `g++ -std=c++14 -Wall -Werror=vla -MMD -c` on all the `.cc` files in the repo  to produce the object file.
Once `make` finishes building all the files,  user should be able to start the game by executing `./cc3k` in the terminal.

## Gameplay
The objective of the game is to cross 5 floors to reach victory and score as many points as possible by collecting gold. Gold is represented by `G` on the board and can be picked up by the user by walking on to that cell. You character is represented on the board by `@` symbol. After every move the status at the bottom will describe what action just happened. The potions, denoted by `P` and gold does not move but the computer generated characters can move randomly within one block of their original position in any direction. 

![Gold](https://raw.githubusercontent.com/angad-singh/cc3k/master/images/gold.png)

Portal to the next floor is represented by  `\` on the board. Users can walk into it to advance to the next level.

After executing `./cc3k` in the terminal, users will be presented with the following options:

![Welcome Screen](https://github.com/angad-singh/cc3k/images/start.png)

Users can choose `s` for Shade, `d` for Drow, `v` for Vampire, `t` for Troll and `g` for Goblin as their race. 

### Movement
Users can move around the board by entering the following command:
`no` for North
`so` for South
`we` for West
`ea` for East
`ne` for North-East
`se` for South-East
`sw` for South-West
`nw` for North-West

### Using potions
Users can walk right adjacent to a potion denoted by `P` on the board can use it by typing `u <dir>` where `<dir>` can be any one of the directions mentioned above.

![Using potions](https://github.com/angad-singh/cc3k/images/potion.png)

### Attacking
Users can attack computer generated characters by walking up to them and passing in the command `a <dir>` where the `<dir>` can be any one of the directions mentioned above. The success of attack is probabilistic and it can be a hit or miss.

![Attacking](https://github.com/angad-singh/cc3k/images/attack.png)
