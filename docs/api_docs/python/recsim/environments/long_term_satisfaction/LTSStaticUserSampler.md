<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="recsim.environments.long_term_satisfaction.LTSStaticUserSampler" />
<meta itemprop="path" content="Stable" />
<meta itemprop="property" content="__init__"/>
<meta itemprop="property" content="get_user_ctor"/>
<meta itemprop="property" content="reset_sampler"/>
<meta itemprop="property" content="sample_user"/>
</div>

# recsim.environments.long_term_satisfaction.LTSStaticUserSampler

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/environments/long_term_satisfaction.py">View
source</a>

## Class `LTSStaticUserSampler`

Generates user with identical predetermined parameters.

Inherits From:
[`AbstractUserSampler`](../../../recsim/user/AbstractUserSampler.md)

<!-- Placeholder for "Used in" -->

<h2 id="__init__"><code>__init__</code></h2>

```python
__init__(
    *args,
    **kwargs
)
```

Creates a new user state sampler.

## Methods

<h3 id="get_user_ctor"><code>get_user_ctor</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/user.py">View
source</a>

```python
get_user_ctor()
```

Returns the constructor/class of the user states that will be sampled.

<h3 id="reset_sampler"><code>reset_sampler</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/user.py">View
source</a>

```python
reset_sampler()
```

<h3 id="sample_user"><code>sample_user</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/environments/long_term_satisfaction.py">View
source</a>

```python
sample_user()
```

Creates a new instantiation of this user's hidden state parameters.
