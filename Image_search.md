# Image Search Fine Tuning

## Silhouette Augmentation
Take the product image → convert to a black & white silhouette:

object = white

background = black

This removes texture/color and leaves pure shape.

## Edge Augmentation

![images/user_query_1.jpg](images/user_query_1.jpg)
![images/edge_map_1.png](images/edge_map_1.png)

edge(customer_image) ↔ edge(product_image)



## Logo crop augmentations
brand cues

# Hard Negatives
- Same category wrong model
- Same color wrong shape
- Same brand wrong model
- “User didn’t click” pairs (gold negatives)
