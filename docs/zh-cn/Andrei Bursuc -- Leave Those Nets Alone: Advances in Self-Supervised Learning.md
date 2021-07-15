# Leave Those Nets Alone: Advances in Self-Supervised Learning



## 1. Motivation

Deep learning requires *large amounts* of *carefully labeled data* which is **difficult to acquire** and **expensive to annotate**.

- difficult to acquire and curate large human-annotated dataset
  - time costly
  - prone to human error
- difficult to keep the pace with an ever changing world
  - data distribution shift all the time e.g. fashion trends
  - infeasible to launch large annotation compaigns each time
- supervised method has blind-spots to learn useful and rich representations
  - acquiring unlabeled data is easy
  - typically cannot exploit these large amount of data

-  The supervision signal can bias the network in unexpected ways.
- Inspiring success of self-supervisison in NLP e.g. mask prediction, next sentence prediction.

Improving representation learning requires features that are not specialised for solving a particular supervised task, but rather *encapsulate richer statistics for various downstream tasks*.



## 2. Self-supervision

- A form of unsupervised learning where the **data** provides the supervision signal.
- Usually, define a **pretext task** for which the network is forced to learn.
- For most pretext tasks, *a part of the data is withheld* and the network has to predict it.
-  The representations learned on the pretext task are used for downstream tasks with annotations.

Evaluation pipeline:

- linear classification
- annotation efficient learning
- transfer learning