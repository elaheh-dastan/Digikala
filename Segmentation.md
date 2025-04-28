# User/Product Segmentation

🎯 Goal
Segment users and products to enable:

1. Personalized recommendations
2. Better UX (search, homepage, promotions)
3. Targeted marketing
4. Strategic decision-making (what products to invest more in, etc.)

📚 Techniques
Simple
1. RFM (good for initial user segmentation)
  - Recency: How recently a user made a purchase.
  - Frequency: How often they purchase.
  - Monetary: How much money they spend.
2. k-Means clustering (unsupervised, simple)
3. Hierarchical clustering

More advanced:
1. DBSCAN (density-based clustering, good if you expect "outlier" groups)
2. Autoencoders + clustering (learn latent features first)
3. Graph-based methods (especially if you have user-product interaction graphs)
4. Self-supervised learning to embed users/products into a low-dim space and cluster

🧠 Deep Diver

Semantic Search

We already have product embedding and add business features, we can add the product cluster to the vector the same way, and when the user searches for something we also define the user's product cluster interest and then search in the Qd or we can search exctly like before and just rerank using this cluster interest.

