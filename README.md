# Conway's Reverse Game of Life
<img width="1900" height="400" alt="image" src="https://github.com/user-attachments/assets/19bbc8c1-5c3b-413a-b17d-2d18a85d3a84" />

# Description
The Game of Life is a cellular automaton created by mathematician John Conway in 1970. The game consists of a board of cells that are either on or off. One creates an initial configuration of these on/off states and observes how it evolves. There are four simple rules to determine the next state of the game board, given the current state:
1. Any live cell with fewer than two live neighbors dies, as if by underpopulation.
2. Any live cell with two or three live neighbors lives on to the next generation.
3. Any live cell with more than three live neighbors dies, as if by overpopulation.
4. Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

These simple rules result in many interesting behaviors and have been the focus of a large body of mathematics.  As Wikipedia tells it:
Ever since its publication, Conway's Game of Life has attracted much interest, because of the surprising ways in which the patterns can evolve. Life provides an example of emergence and self-organization. It is interesting for computer scientists, physicists, biologists, biochemists, economists, mathematicians, philosophers, generative scientists and others to observe the way that complex patterns can emerge from the implementation of very simple rules. The game can also serve as a didactic analogy, used to convey the somewhat counter-intuitive notion that "design" and "organization" can spontaneously emerge in the absence of a designer. For example, philosopher and cognitive scientist Daniel Dennett has used the analogue of Conway's Life "universe" extensively to illustrate the possible evolution of complex philosophical constructs, such as consciousness and free will, from the relatively simple set of deterministic physical laws governing our own universe.

The emergence of order from simple rules begs an interesting question -- what happens if we set time backwards?

This competition is an experiment to see if machine learning (or optimization, or any method) can predict the game of life in reverse.  Is the chaotic start of Life predictable from its orderly ends?  We have created many games, evolved them, and provided only the end boards. You are asked to predict the starting board that resulted in each end board. Although some people have examined this problem, it is unknown (at least, to us...) just how difficult this will be.

# Evaluation
You are evaluated on the mean absolute error of your predictions. In this case, this is equivalent to 1 - (classification accuracy). You may only predict 0 (dead) or 1 (alive) for each cell.

# Submission File
For every game in the test set, your submission file should list the predicted starting board on a single row.  Values are listed in a column-wise order. That is, if you want to predict a matrix,
<img width="660" height="53" alt="image" src="https://github.com/user-attachments/assets/03173366-9cf0-48e5-ab63-ad2780cf6b47" />

the predicted row would be (1,3,2,4). The submission file should contain a header and have the following format:
<img width="659" height="94" alt="image" src="https://github.com/user-attachments/assets/f3223922-001e-426a-b0de-20170c679c18" />

