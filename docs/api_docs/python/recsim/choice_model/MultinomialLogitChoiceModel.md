<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="recsim.choice_model.MultinomialLogitChoiceModel" />
<meta itemprop="path" content="Stable" />
<meta itemprop="property" content="score_no_click"/>
<meta itemprop="property" content="scores"/>
<meta itemprop="property" content="__init__"/>
<meta itemprop="property" content="choose_item"/>
<meta itemprop="property" content="score_documents"/>
</div>

# recsim.choice_model.MultinomialLogitChoiceModel

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/choice_model.py">View
source</a>

## Class `MultinomialLogitChoiceModel`

A multinomial logit choice model.

Inherits From:
[`NormalizableChoiceModel`](../../recsim/choice_model/NormalizableChoiceModel.md)

<!-- Placeholder for "Used in" -->

Samples item x in scores according to p(x) = exp(x) / Sum_{y in scores} exp(y)

#### Args:

*   <b>`choice_features`</b>: a dict that stores the features used in choice
    model: `no_click_mass`: a float indicating the mass given to a no click
    option.

<h2 id="__init__"><code>__init__</code></h2>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/choice_model.py">View
source</a>

```python
__init__(choice_features)
```

Initialize self. See help(type(self)) for accurate signature.

## Properties

<h3 id="score_no_click"><code>score_no_click</code></h3>

<h3 id="scores"><code>scores</code></h3>

## Methods

<h3 id="choose_item"><code>choose_item</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/choice_model.py">View
source</a>

```python
choose_item()
```

Returns selected index of document in the slate.

#### Returns:

*   <b>`selected_index`</b>: a integer indicating which item was chosen, or None
    if none were selected.

<h3 id="score_documents"><code>score_documents</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/choice_model.py">View
source</a>

```python
score_documents(
    user_state,
    doc_obs
)
```

Computes unnormalized scores of documents in the slate given user state.

#### Args:

*   <b>`user_state`</b>: An instance of AbstractUserState.
*   <b>`doc_obs`</b>: A numpy array that represents the observation of all
    documents in the slate.

#### Attributes:

*   <b>`scores`</b>: A numpy array that stores the scores of all documents.
*   <b>`score_no_click`</b>: A float that represents the score for the action of
    picking no document.
