## Patch Evolution Study

 👋
This is a supplementary repository for paper submission "**Unveiling the Characteristics and Impact of Security Patch Evolution**".
In this study, we take the first look to systematically investigate the phenomenon of security patch evolution in open-source projects. In particular, we performed extensive experiments on a large-scale dataset containing 1,046 distinct CVEs with 2,633 patches collected from popular open-source projects (e.g., linux, openssl).


This project currently contains supplementary materials for the paper, especially a cleaned dataset we used for patch evolution tracking. 
In detail, each pickle file in [dataset](dataset/) holds information related to its respective project such as CVEs, patches, and all versions of the patch-related functions.



## Dataset Usage

We extracted the mate data of each patch and all evolved patch-related functions.
The pickle file also records other necessary information for this study, including the name of patch-related file/functions, timestamp, authorship, commit massage et al.


```Python
import pickle
with open('dataset/Evo_FFmpeg.pkl', 'rb') as f:
    pkl = pickle.load(f)

```