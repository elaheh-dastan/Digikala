# Latent Dirichlet Allocation

## Problem
We have a few corpuses and we want to find out their topics.

LDA takes a geometric approach.

![images/LDA.png](images/LDA.png)

![images/best_setting.png](images/best_setting.png)

![images/blueprint.png](images/blueprint.png)

![images/setting.png](images/setting.png)

![images/setting_2.png](images/setting_2.png)

![images/alpha.png](images/alpha.png)

![images/dist_of_dist.png](images/dist_of_dist.png)

In the image above, the corners are topics and the points inside are DOCUMENTS.

![images/dirichle_distributions.png](images/dirichle_distributions.png)

![images/latentDA.png](images/latentDA.png)

This formula calculates the probability that a particular document comes out of the machine

![images/LDA_formula.png](images/LDA_formula.png)

![images/LDA_formula_image.png](images/LDA_formula_image.png)


From alpha we get theta, from beta we get thai.

![images/LDA_formula_graph.png](images/LDA_formula_graph.png)

We combine zed and thai to obtain a list of words, one word per topic. We concatenate these words to obtain a document and then we do this as many times as number of documents in the corpus.
