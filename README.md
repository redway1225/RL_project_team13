# Replication: Multi-Step Reinforcement Learning: A Unifying Algorithm

> This is a replication of the algorithm mentioned in (Asis et al. 2017) 

There are many environments and algorithms in Reinforcement Learning (RL). In value based RL, TD(λ) unifies the Monte Carlo method(update per episode) and the Temporal difference method(update per steps) by using λ to control the trade-offs of them. SARSA and Tree-backup(use expected SARSA in each step) are two different ways of computing TD target, which the former is using full sampling and the later is using pure expectation to estimate this value.
These two algorithms performed in multi-steps case are not dominated the others for all problems, so this paper performed a multi-steps algorithm called Q(σ) which merges them by using an variable σ which controls the trade-offs of using SARSA and Tree-backup.

Implemented algorithms:

# Curves (commit `````)

## 19-state Random Walk Example: n-step TD Prediction

![Loading...](https://github.com/redway1225/RL_project_team13/blob/master/image/19-state%20Random%20Walk%20.png?raw=true)  
n : 1→16  
α : 0→1  
σ : { 0 , 0.25 , 0.5 , 0.75 , 1 } , and dynamic decreasing σ from 1 to 0  
episode : 50 episodes  
result : Averaged across 100 runs  

## Stochastic Windy Gridworld

![Loading...](https://raw.githubusercontent.com/redway1225/RL_project_team13/master/image/Stochastic%20windy%20gridworld.png?token=AE2SDJDS3OGH5PHFMNNWSS27CESWI)  
ε-greedy policy, ε : 0.1  
n : 1 and 3  
α : 0 -> 1  
σ : { 0 , 0.5 , 1 } , and dynamic decreasing σ from 1 to 0   
episode : 100 episodes in experiment  
result : Averaged across 1000 runs

## 19-state Random Walk Example: n-step TD Prediction

![Loading...](https://github.com/redway1225/RL_project_team13/blob/master/image/19-state%20Random%20Walk%20.png?raw=true)  
n : 1→16  
α : 0→1  
σ : { 0 , 0.25 , 0.5 , 0.75 , 1 } , and dynamic decreasing σ from 1 to 0  
episode : 50 episodes  
result : Averaged across 100 runs  
