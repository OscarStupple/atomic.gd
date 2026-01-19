This is an atomic scale, n-body, classical simulation of all* the fundamental forces, based in godot.

This is the first part of a series of simulations, working toward the most accurate and powerful model, that aim to capture the inner workings of the smallest scales.
This was also developed as my Extended Project Qualification, therefore many decisions were made in aid of the time and achievability of the project.

I intend to follow this with:
Another classical simulation using python and/or c++, that aims to improve upon this by having more time, better efficiency, and will make use of some publicly available tools.
A non-classical, sub-atomic scale simulation, based more strongly in the standard model.

Currently the program is set to run, a pre-determined exemplar.
Proper use of the simulation for testing and capture requires utilising godot’s game engine (by dragging in and moving particles) in the 3d editor. This is both impractical and improper so is a feature that I intend to add (if I ever push a full release), alternatively it will be improved upon in later iterations of the project.

Operation, Features, and Function:
---------------------------------

The program runs pairwise calculations of forces and sums the force vectors for each particle before determining the subsequent motion.

The fundamental forces of this simulation are:

Electromagnetism – via the Lorentz force

Residential Nuclear force – via the Yukawa potential

Gravity – via General Universal Gravitation

Later releases include hadronic particle interactions.

The two most significant emergent behaviours from this program have been nuclei formation and nucleon drip.

Those intrigued in this project may be interested by particle.js by Andre Nepomuceno, the inspiration for the form this simulation takes, and generally a quite impressive, and visually interesting program.
