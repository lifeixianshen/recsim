<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="recsim.environments.long_term_satisfaction.clicked_engagement_reward" />
<meta itemprop="path" content="Stable" />
</div>

# recsim.environments.long_term_satisfaction.clicked_engagement_reward

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/environments/long_term_satisfaction.py">View
source</a>

Calculates the total clicked watchtime from a list of responses.

```python
recsim.environments.long_term_satisfaction.clicked_engagement_reward(responses)
```

<!-- Placeholder for "Used in" -->

#### Args:

*   <b>`responses`</b>: A list of LTSResponse objects

#### Returns:

*   <b>`reward`</b>: A float representing the total watch time from the
    responses
