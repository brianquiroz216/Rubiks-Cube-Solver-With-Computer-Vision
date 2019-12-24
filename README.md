# Rubiks-Cube-Solver-With-Computer-Vision
Given an image of each face of a Rubik's cube, detect the cube, classify its stickers' colors, and output a solution algorithm

## Instructions
- There are two ways of running this program:
    - Use the detector program to determine the cube configuration and pass it on to the solver program (auto scramble)
    - Input your own scramble algorithm to the solver program (manual scramble)

## Auto Scramble
1. Take 6 images of a Rubik's cube, one of each side, and name each face's picture according to the following convention:
    - yellow face: Img1.jpg
    - orange face: Img2.jpg
    - blue face: Img3.jpg
    - red face: Img4.jpg
    - green face: Img5.jpg
    - white face: Img6.jpg

2. Store the folder containing these images under Detector/Images.

3. Go to Detector/CVRubiksCube.m and change "ExampleSet" on line 2 for your folder's name.

4. Open MATLAB and run the CVRubiksCube.m script in the Detector folder. This should create a file called "stickers.txt" in that folder.

5. Go to Solver and make to generate the .o files and the executable for the solver.

6. On the command line, run:
    `./RubiksCubeSolver auto`
    
    The C++ program should now output the scrambled cube, each step it performed, and a series of steps you can use to solve the cube in that state.
 
## Manual Scramble
1. Go to Solver and make to generate the .o files and the executable for the solver.
2. On the command line, run:
    `./RubiksCubeSolver manual`
    
    The C++ program should now output the scrambled cube, each step it performed, and a series of steps you can use to solve the cube in that state.
    
## Further Documentation
This project is a combination of two separate projects the detector and the solver. I added some code to make them work together in this repository.
To learn more about each, you can view the code for each component in their respective repository:
- Detector: https://github.com/brianquiroz216/Rubiks-Cube-Recognition-and-Color-Classification
- Solver: https://github.com/brianquiroz216/Rubiks-Cube-Solver

