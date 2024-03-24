This is the repository containing the numerical experiments in a paper by me and Ziping,
"A Natural Extension To Online Algorithms For Hybrid RL With Limited Coverage", 
which you can find at https://arxiv.org/abs/2403.09701.

The simulations demonstrate that appending offline data to the experience replay buffer 
can encourage sufficient exploration for the portion of the state-action space that does not have good coverage.
Doing so leads to a simple, but effective, extension of an online RL algorithm to the setting of hybrid RL.

That is, where the "offline partition" is the portion of the state-action space well-visited by the behavior policy,
and the "online partition" is its complement, We see that the hybrid RL algorithm visits the online partition more often than the online RL algorithm,
and vice-versa for the offline partition. This happens in both a tabular forest management simulator, and a Tetris simulator we cast as a linear MDP.

<img width="1137" alt="Screenshot 2024-03-24 at 7 56 15 PM" src="https://github.com/hetankevin/hybridcov/assets/55823167/e9b5b107-4307-4bd3-bc3c-e597ade220cf">

<img width="1151" alt="Screenshot 2024-03-24 at 7 56 37 PM" src="https://github.com/hetankevin/hybridcov/assets/55823167/9f9de815-0776-4e98-b4d0-30cc1acfc9cf">

<img width="820" alt="Screenshot 2024-03-24 at 7 57 57 PM" src="https://github.com/hetankevin/hybridcov/assets/55823167/f717fa23-a704-42da-88db-5893fded547c">


