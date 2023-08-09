# DinoDash

Final project for EE319K (Intro to Embedded Systems).

The youtube link here showcases the game in action as well as describes how it was made.
[https://youtu.be/9Rm7kBxFm9c]

The task was to create a video game using the embedded system practices learned over the course of the semester. I designed a replication of the Google Dinosaur game that is played when there is no internet connection available, however my version allows for user movement and to shoot a laser to destroy incoming enemies. The game uses two buttons as an input, one to shoot a laser and one to jump to avoid obstacles. A 4-bit DAC is utilized with an interrupt timer to play sound when a user inputs a command, such as the jump and shoot described.

The LED board is continuosly updated using a Systick Timer that interrupts the program and detect positions of the objects and possible collisions that would end the game or destroy an enemy. During this Systick interrupt at 16MHz, the slide potentiometer is read to detect the position of the character on the screen.

The game goes on forever or until the user is struck by an enemy, which would lead them to the menu screen to start again.

The game is coded in C/C++ and ARM Cortx-M assembly language and is available to play in English and German.

Skills learned/used: C/C++, ARM Cortex-M assembly, ADC/DAC, System Interrupts, Game Design, OOP, Embedded Systems basics.
