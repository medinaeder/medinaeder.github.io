“Do a kickflip!” Tony yelled at the humanoid. At this point I had seen them walking around, doing cartwheels, unloading dishwashers, folding laundry, and swinging like spiderman. This one was eyeing(lidaring) a skateboard. These robots were designed to be fully autonomous. Not rigid machines but explorers, learners, capable of adapting to the world.  They had never interacted with objects that humans used for leisure other than to put them away. The humanoid knew how to traverse unsteady terrain but it couldn’t ride a bike. It had never experienced fun. No one had built that simulator yet. 

But the robot was curious. Riding on the board would probably take a few shots but not that many more. Walking on unsteady terrain had been its training data. It was a nearby extrapolation. Just another wobbly surface underfoot. The accelerometers would feel an initial jerk and respond, trying to stabilize. Learning to push off? A little trickier but it’s not that different than walking.

We’ve already seen them manipulate objects with nearly dexterous hands. But a kickflip seems harder. Maybe it isn’t. Maybe it’s like flipping a pen. Or it’s the same as jumping. But something in me screams that planning foot motion on an unsteady dynamic surface to create a skateboard to flip in mid air is just too difficult. The type of problem that is always worth it. 

What about the morphology? Can you do a kickflip with limited ankle mobility? Can you do a kickflip in ski boots?

How would I first attempt this problem:
- Understand the problem
    - Ask a Language model for a set of reduced skateboard dynamics 
    - Read existing simplified skateboard dynamics models
- Collect Human Data
    - Record high-speed video using mocap 
    - Generate digital rig and track angles
    - Track board position, orientation, angular velocity 
- Model and Simulate
    - Build physics-based simulation
    - Use behavior cloning to imitate human motion
    - Apply RL to improve the board flip motion
    - Use curriculum learning: ollies to flip
    - Focus Areas
        - Pop: Teach robot how to generate vertical force on tail while balanced
        - Catch and Land: Simple ollie safely
        - Flip: Train foot motion to add spin
- Physical Transfer
    - Build a robot. Spongebob draws a circle. 
    - Iterate

—
Sources 
[Skateboard physics explained](https://www.youtube.com/watch?v=OxV-u-WnbW4) 
[Skateboard dynamics model](https://www.sciencedirect.com/science/article/abs/pii/0045782595009329) 
[Ollie Model](https://engrxiv.org/preprint/download/3171/version/4465/5768/4565)
[Mujoco](https://mujoco.org/) 
[NVidia Isaac](https://developer.nvidia.com/isaac/sim) 
[Imitation Learning - behavior cloning](https://imitation.readthedocs.io/en/latest/algorithms/bc.html) 

