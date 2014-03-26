HTML5 Genetic Cars
==================

A genetic algorithm car evolver in HTML5 canvas.

This is inspired by BoxCar2D, and uses the same physics engine, Box2D, but it's written from scratch.

This is the code as published on http://rednuht.org/genetic_cars_2/


Controls

Suprise: Toggles drawing, makes the simulation faster.
New Population: Keeps the generated track and restarts the whole car population.
Create new world with seed: The same seed always creates the same track, so you can agree on a seed with your friends and compete. :)
Mutation rate: The chance that each gene in each individual will mutate to a random value when a new generation is born.
Mutation size: The range each gene can mutate into. Lower numbers mean the gene will have values closer to the original.
Floor: If set to mutable, a new terrain will be generated each round.
Gravity: Enjoy the freedom of driving on the moon, you cheater!
Elite clones: The top n cars that will be copied over to the next generation.
View top replay: Pause the current simulation and show the top performing car. Click a second time to resume simulation.
Graph

Red: Top score in each generation.
Green: Average of the top 10 cars in each generation.
Blue: Average of the entire generation.
But what is it?

The program uses a simple genetic algorithm to evolve random two-wheeled shapes into cars over generations. Loosely based on BoxCar2D, but written from scratch, only using the same physics engine (box2d).
seedrandom.js written by David Bau. (thanks!)
Genome

The genome consists of:
- Shape: (8 genes, 1 per vertex)
- Wheel size: (2 genes, 1 per wheel)
- Wheel position: (2 genes, 1 per wheel)
- Wheel density: (2 genes, 1 per wheel) darker wheels mean denser wheels
- Chassis density: (1 gene) darker body means denser chassis
Blurb

This is not as deterministic as it should be, so your best car may not perform as well as it once did. The terrain gets more complex with distance.
