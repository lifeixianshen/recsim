<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="recsim.environments.interest_evolution.IEvVideoSampler" />
<meta itemprop="path" content="Stable" />
<meta itemprop="property" content="num_clusters"/>
<meta itemprop="property" content="__init__"/>
<meta itemprop="property" content="get_doc_ctor"/>
<meta itemprop="property" content="reset_sampler"/>
<meta itemprop="property" content="sample_document"/>
</div>

# recsim.environments.interest_evolution.IEvVideoSampler

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/environments/interest_evolution.py">View
source</a>

## Class `IEvVideoSampler`

Class to sample interest_evolution videos.

Inherits From:
[`AbstractDocumentSampler`](../../../recsim/document/AbstractDocumentSampler.md)

<!-- Placeholder for "Used in" -->

<h2 id="__init__"><code>__init__</code></h2>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/environments/interest_evolution.py">View
source</a>

```python
__init__(
    doc_ctor=recsim.environments.interest_evolution.IEvVideo,
    min_feature_value=-1.0,
    max_feature_value=1.0,
    video_length_mean=4.3,
    video_length_std=1.0,
    **kwargs
)
```

Creates a new interest evolution video sampler.

#### Args:

*   <b>`doc_ctor`</b>: A class/constructor for the type of videos that will be
    sampled by this sampler.
*   <b>`min_feature_value`</b>: A float for the min feature value.
*   <b>`max_feature_value`</b>: A float for the max feature value.
*   <b>`video_length_mean`</b>: A float for the mean of the video length.
*   <b>`video_length_std`</b>: A float for the std deviation of video length.
*   <b>`**kwargs`</b>: other keyword parameters for the video sampler.

## Properties

<h3 id="num_clusters"><code>num_clusters</code></h3>

Returns the number of document clusters. Returns 0 if not applicable.

## Methods

<h3 id="get_doc_ctor"><code>get_doc_ctor</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/document.py">View
source</a>

```python
get_doc_ctor()
```

Returns the constructor/class of the documents that will be sampled.

<h3 id="reset_sampler"><code>reset_sampler</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/document.py">View
source</a>

```python
reset_sampler()
```

<h3 id="sample_document"><code>sample_document</code></h3>

<a target="_blank" href="https://github.com/google-research/recsim/tree/master/recsim/environments/interest_evolution.py">View
source</a>

```python
sample_document()
```

Samples and return an instantiation of AbstractDocument.
