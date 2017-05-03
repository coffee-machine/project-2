# Project 2 - Rush Hour

Rush Hour is a [board game](https://en.wikipedia.org/wiki/Rush_Hour_\(board_game\)) played on a 6x6 area. The goal is to get the red car to the exit. In total there are 12 cars of length 2 and 4 trucks of length 3. The board is set up according to placement of cars and trucks on puzzle cards.

## Bureaucratic Information

* Each group should submit a short, clear report on the intranet by the stated deadline. **Late submissions will not be accepted.**
* The solutions of different groups must be independent and sharing parts of the code or the text of the report is **strictly forbidden**.
* The project will account for 30% of your final mark for the course.
* The deadline for delivering the project report is **Thursday, 11 May 2017, at 23:59 GMT**.

## Literature
* F.W. Vaandrager [A First Introduction to Uppaal](http://www.mbsd.cs.ru.nl/publications/papers/fvaan/handbookuppaal/). In J. Tretmans, editor. Quasimodo Handbook. To appear. (The link also points to files with the models mentioned in the book chapter.)
* [A Tutorial on UPPAAL](http://www.it.uu.se/research/group/darts/papers/texts/new-tutorial.pdf).

## About the project

Before you start working on the project, you should
* have read the above-mentioned literature, and
* have installed and can run [Uppaal](http://www.uppaal.org/) on your laptop.

You are asked to provide a brief and clear report describing how you solved the tasks below. The report should be delivered as a PDF document.

Your tasks are as follows.

1. In this exercise you are asked to model the solitaire game RUSH HOUR and use UPPAAL to solve the puzzle. The game is simple. You have a 6x6 board like the one shown on the picture to be found [here](http://www.ru.is/faculty/luca/MV09SPRING/rush.png). On the board you find a number of vehicles of different size (cars and trucks). The goal of the game is to move the vehicles by driving forward and backwards in such a way that the RED car can leave the board at the exit on the right side of the board. The vehicles cannot turn!
2. Make a model of the game in UPPAAL. Hint: you may want to model each (type of) vehicle as an automaton (template), where a vehicle can only move one position at a time. Also, you could use a two-dimensional bit-array to represent information about locations on the board that are currently occupied.
3. Using your model and the model checker of UPPAAL solve the two puzzles shown in the picture [here](http://www.ru.is/faculty/luca/MV09SPRING/puzzle.jpg). What is the shortest number of steps/moves needed to solve the puzzle?
4. Can you use UPPAAL to solve the game for (one of) the two hard configurations given [here](http://quomodocumque.wordpress.com/2012/02/18/the-hardest-rush-hour-position/)?
5. Extend your model with timing constraint.
	* First assume that it takes 5 seconds to move a truck and 2 seconds to move a car.
	* (Bonus assignment) Next, assume that you have two hands, so that you potentially can move two vehicles (one position) simultaneously. Furthermore assume that you are left-handed so that it takes 3 seconds to move a vehicle one position with the left hand but 5 seconds to move a vehicle one position with the right hand.

In both cases, use Uppaal to find the fastest way of solving the puzzle (not measured in computation time, but in terms of the overall time that it takes to move all the vehicles). Tip: Use UPPAAL's diagnostic trace feature and ask for the fastest trace.
6. Use (and describe) the resulting message sequence charts for illustrating the solutions.
7. Finish your report by briefly commenting on what was your experience working with the tool.
8. Compile a single PDF file and post the file on the intranet by the stated deadline.