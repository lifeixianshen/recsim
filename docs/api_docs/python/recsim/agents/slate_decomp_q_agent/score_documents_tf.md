<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="recsim.agents.slate_decomp_q_agent.score_documents_tf" />
<meta itemprop="path" content="Stable" />
</div>

# recsim.agents.slate_decomp_q_agent.score_documents_tf

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/agents/slate_decomp_q_agent.py">View
source</a>

Computes unnormalized scores given both user and document observations.

```python
recsim.agents.slate_decomp_q_agent.score_documents_tf(
    user_obs,
    doc_obs,
    no_click_mass=1.0,
    is_mnl=False,
    min_normalizer=-1.0
)
```

<!-- Placeholder for "Used in" -->

This implements both multinomial proportional model and multinormial logit model
given some parameters. We also assume scores are based on inner products of
user_obs and doc_obs.

#### Args:

*   <b>`user_obs`</b>: An instance of AbstractUserState.
*   <b>`doc_obs`</b>: A numpy array that represents the observation of all
    documents in the candidate set.
*   <b>`no_click_mass`</b>: a float indicating the mass given to a no click
    option
*   <b>`is_mnl`</b>: whether to use a multinomial logit model instead of a
    multinomial proportional model.
*   <b>`min_normalizer`</b>: A float (<= 0) used to offset the scores to be
    positive when using multinomial proportional model.

#### Returns:

A float tensor that stores unnormalzied scores of documents and a float tensor
that represents the score for the action of picking no document.
