# Membership Inference Attacks on Sequence-to-Sequence Models

https://arxiv.org/abs/1904.05506

Sorami Hisamoto, Matt Post, Kevin Duh

<img src="figures/alice_and_bob.png" width="600px">


## Data

## Corpus

<img src="figures/data_and_splits.png" width="600px">

For our experiment, we had 5 main subcorpora. We used corpora from the Conference on Machine Translation (WMT18) ([Bojar et al., 2018](https://www.aclweb.org/anthology/W18-6401/)). 

Carol, the judge, gives Alice 4 subcorpora as her MT model training data, namely `CommonCrawl`, `Europarl v7`, `News Commentary v13`, and `Rapid 2016`. Carol excludes 5,000 samples from each training sets as *out probes*, and select 5,000 samples within the training sets as *in probes*. 

Bob gets a subset of the data Alice has, excluding Alice *in probes*. He can use this data in whatever way he wants for his attack.

In addition, Carol gives Alice `ParaCrawl`, but not to Bob. We can think of it  as an in-house data the MT service provider holds. 



## Out-of-domain Subcorpora

Additionally, we have 4 out-of-domain (OOD) subcorpora, namely `EMEA` and `Subtitles 18` ([Tiedemann, 2012](https://www.aclweb.org/anthology/L12-1246/)), `Koran` (Tanzil), and `TED` ([Duh, 2018](http://www.cs.jhu.edu/~kevinduh/a/multitarget-tedtalks/)).


## Size

<img src="figures/data_size.png" width="800px">

