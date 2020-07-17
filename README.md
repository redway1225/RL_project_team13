# Replication: Multi-Step Reinforcement Learning: A Unifying Algorithm

> This is a replication of the algorithm mentioned in (Asis et al. 2017) 

There are many environments and algorithms in Reinforcement Learning (RL). In value based RL, TD(λ) unifies the Monte Carlo method(update per episode) and the Temporal difference method(update per steps) by using λ to control the trade-offs of them. SARSA and Tree-backup(use expected SARSA in each step) are two different ways of computing TD target, which the former is using full sampling and the later is using pure expectation to estimate this value.
These two algorithms performed in multi-steps case are not dominated the others for all problems, so this paper performed a multi-steps algorithm called Q(σ) which merges them by using an variable σ which controls the trade-offs of using SARSA and Tree-backup.

Implemented algorithms:
