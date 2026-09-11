This is an atomic scale, n-body, classical simulation of all* the fundamental forces, based in godot.

This is the first part of a series of simulations, working toward an accurate and powerful model, that aims to capture the inner workings of the smallest scales.
This was also developed as my Extended Project Qualification, therefore many decisions were made in aid of the time and achievability of the project.

I intend to follow this with:
Another classical simulation using python and/or c++, that aims to improve upon this by leveraging more resources, better efficiency, and will make use of some external tools.
Then a non-classical, sub-atomic scale simulation, based more strongly in the standard model.

Currently the program is set to randomly distribute 50 protons and 50 neutrons in a small area localised around the camera.
Proper use of the simulation for testing and capture requires utilising godot’s game engine (by dragging in and moving particles) in the 3d editor. This is both impractical and improper so is a feature that I intend to add (if I ever push a full release).

Operation, Features, and Function:
---------------------------------

The program runs pairwise calculations of forces and sums the force vectors for each particle before determining the subsequent motion.

The fundamental forces of this simulation are:

Electromagnetism – via the Lorentz force

Residential Nuclear force – via the Yukawa potential

Gravity – via General Universal Gravitation

Later releases include hadronic particle interactions.

Time Manipulation - using the arrow keys, and spacebar, increase, decrease, reverse, or pause the speed of the simulation. Note that larger time steps are less accurate and reversed time is currently experimental only.

The two most significant emergent behaviours from this program have been nuclei formation and nucleon drip.

Those intrigued in this project may be interested by particle.js by Andre Nepomuceno, the inspiration for the form this simulation takes, and generally a quite impressive, and visually interesting program.
