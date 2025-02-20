<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="recsim.agents.agent_utils.epsilon_greedy_exploration" />
<meta itemprop="path" content="Stable" />
</div>

# recsim.agents.agent_utils.epsilon_greedy_exploration

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/agents/agent_utils.py">View
source</a>

Epsilon greedy exploration.

```python
recsim.agents.agent_utils.epsilon_greedy_exploration(
    state_action_iterator,
    q_function,
    epsilon
)
```

<!-- Placeholder for "Used in" -->

Either picks a slate uniformly at random with probability epsilon, or returns a
slate with maximal Q-value. TODO(mmladenov): more verbose doc. Args:
state_action_iterator: an iterator over slate, state_action_index tuples.
q_function: a container holding Q-values of state-action pairs. epsilon:
probability of random action. Returns: slate: the picked slate. sa_index: the
index of the picked slate in the Q-value table.
