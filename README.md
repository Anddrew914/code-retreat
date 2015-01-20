![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Ruby \& RSpec Lab: Code Retreat

## Objectives

By the end of this, students should be able to:

- Pair with other students in a ping-pong, test-driven style.
- Explain the value of team communication and test-driven development in their own words.
- Solve a problem in multiple ways by "spiking".
- Choose an implementation strategy for a problem using lessons learned from spikes.

## Instructions

This code retreat will consist of four to five pairing rounds. Try to pair with someone new each time. For each round, you and your pair will work on implementing Conway's Game of Life in ruby (see below). After each round we will hold a quick retrospective to share our experiences with each other.

We'll complete the following activities. With the exception of the first, they should all be practiced test-first:

- Caveman Coder (30 minutes)
- Ping-pong (45 mintues)
- Silent Coder (45 mintues)
- Small Methods (45 mintues)
- Free-for-all (1 hour)

## Notes

### Code Retreat

A code retreat is a day-long intensive practice, focusing on fundamentals. Pairs of programmers tackle the same problem multiple times under different constraints. The constraints are chosen to emphasize the value of modern development practices like test-driven development, pair programming, patterns, and iterative development.

Corey Haines expalins the goals of a code retreat in [Cleveland Code Retreat Introduction on Vimeo](http://vimeo.com/18955165).

### Conway's Game of Life

The Game of Life, also known simply as Life, is a cellular automaton devised by the British mathematician John Horton Conway in 1970.

Visualization of the Game of Life:

![Alt Conway's Game of Life](http://upload.wikimedia.org/wikipedia/commons/e/e5/Gospers_glider_gun.gif)

The "game" is a zero-player game, meaning that its evolution is determined by its initial state, requiring no further input. One interacts with the Game of Life by creating an initial configuration and observing how it evolves.

The universe of the Game of Life is an **infinite two-dimensional orthogonal grid** of square cells, each of which is in one of two possible states, live or dead. Every cell interacts with its eight neighbors, which are the cells that are directly horizontally, vertically, or diagonally adjacent.

#### Rules
At each step in time, the following transitions occur:

1. Any live cell with fewer than two live neighbours dies, as if caused by underpopulation.
2. Any live cell with more than three live neighbours dies, as if by overcrowding.
3. Any live cell with two or three live neighbours lives on to the next generation.
4. Any dead cell with exactly three live neighbours becomes a live cell.

The initial pattern constitutes the seed of the system. The first generation is created by applying the above rules simultaneously to every cell in the seed. **Births and deaths happen simultaneously**, and the discrete moment at which this happens is sometimes called a `tick` (in other words, each generation is a pure function of the one before). The rules continue to be applied repeatedly to create further generations.

## Bonus

If you're looking for extra challenge or practice once you've completed the above, try pairing with someone using the following constraints:

- No mutation of state allowed. Once a variable is assigned, it cannot change.
- No conditionals. Do not use `if/else` and friends.
- No loops.

If you have a working solution you like, post it to GitHub. It's great for employers to see you tackling such a classic problem. Work with a classmate to refactor your code using [SOLID](http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod) and [The Rules of Simple Design](http://xprogramming.com/classics/expemergentdesign/).

## Additional Resources

- [Screencast: Coding Conway’s Game of Life in Ruby the TDD Way with RSpec](http://www.rubyinside.com/screencast-coding-conways-game-of-life-in-ruby-the-tdd-way-with-rspec-5564.html)
