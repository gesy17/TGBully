# TGBully - Temporal Graph-based Cyberbullying Detection

Implementation of <ins>T</ins>emporal <ins>G</ins>raph-based Cyber<ins>bully</ins>ing Detection Model [1].

The TGBully framework consists of three major components:
(1) a semantic context modeling module that encodes each comment by considering both its textual content and user’s language behavior reflected from her/his historical comments, 
(2) a temporal graph interaction learning module that constructs a temporal graph and models the dynamic user interaction with a bully-featured GAT. The proposed GAT jointly captures topic coherence and temporal dynamics in the modeling process; and 
(3) a session classification module that attentively aggregates information from user interaction into a session representation, based on which it then classifies the session into a bullying/non-bullying session.

![Overall Framework](data/model.pdf)

## Code Usage
1. Download all the required data and word embedding files as instructed by the [data README](data/README.md).
 
2. Run the script [Instagram_code.ipynb](Instagram_code.ipynb) and [Vine_code.ipynb](Vine_code.ipynb) for experimental results on the two benchmark datasets.

## Environment
* python == 3.6.7
* cudnn == 7.1.2
* keras == 2.2.4
* numpy == 1.16.4 
* tensorflow-gpu == 1.12.0 

### Reference
> \[1\] [Suyu Ge](https://gesy17.github.io/), [Lu Cheng](http://www.public.asu.edu/~lcheng35/), and [Huan Liu](http://www.public.asu.edu/~huanliu/). Improving Cyberbullying Detection with User Interaction. *The Web Conference (WWW)*, 2021. \[[paper](https://arxiv.org/abs/2011.00449)\]
