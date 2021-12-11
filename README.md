# CS 445: Computational Photography Final Project

## Detecting ASL Alphabet Letters.

Let's see if we can use what we learned from class to detect, in real-time, which letters people are trying to sign in ASL.

## How to Make Training Data

1. Make a new directory in `data/` with the appropriate letter label. Let's do `f` as an example. This would then be: `mkdir data/f/`
2. In the `Sign Language Data Processing` notebook, alter the line that says `letter = __` to be your letter. (Ex. `letter = f`).
3. Click `Kernel -> Restart & Run All`
4. When the camera window opens, hold your hand in the shape of the ASL letter you've chosen in the blue square on screen.
5. Wait for the program counter to take 300 images of your hand in this position.
6. Press the `Esc` key. The program will halt and the window won't close. This is okay.
7. Move all the files with this letter into the appropriate data directory. `mv f* data/f/`.
8. Repeat!

## Running Model

1. In Jupyter notebook, run the file `model.pynb` ensuring that the data is in the correct directory.
3. A random set of letters will be chosen to identify and the percent accuracy will print at the bottom.
