# Udacity Deep Reinforcement Learning: Navigation Report

## Some Important Factors of the Implemented DDPG Algorithm
  1. Actor-Critic Architecture: a combination of the advantages of both Policy-based and Value-based techniques. Actor learns the Optimal Policy, while Critic learns the Value Function to evaluate the Actions of the Actor.
  2. Actor & Critic: are two similar Neural Net architectures, each with three fully connected layers. While Critic has only one output, Actor has the tanh values of the Action Vector.
  3. Target Networks: two sets combining of one Target Actor and one Target Critic that are periodically, softly updated with the weights of the Local Actor and Critic, respectively. 
  4. Soft Updates: gradually blend the Target Network weights with the Local Network weights, preventing oscillations.
  5. Deterministic Policy: making the learning process stable and balancing both Exploration & Exploitation.
  6. Experience Delay: with repetition learning and uncorrelated experience.
  7. Ornstein-Uhlenbeck approach: for processing exploration noise.
  8. The Udacity codebase is modified to handle 20 idential agents.
  9. Hypeparameters:
       The number of units of the network layers is adjusted several times with 400/300, 32/32, 64/64, 128/128, 256/256, then, finally, 128/256 as recommended by Udacity Knowledge.
       Increased the number of time steps to 2368 to hopefully cover a majority of the possibility of States, Actions, & Rewards.
       Utilized the Udacity Project Instructions to add the number of learning updates, and the number of time steps before an update.

## Plot of Rewards

## Ideas for Future Work
Given the codebase, try to implement additional algorithms such as:
  1. PPO
  2. A3C
  3. D4PG
  4. REINFORCE
  5. TNPG
  6. RWR
  7. REPS
  8. TRPO
  9. CEM
  10. CMA-ES
      
Also try to evaluate the effectiveness of these algorithms if possible
