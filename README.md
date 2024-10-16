# Digikala
## Similarity Search, Hierarchical Navigable Small World (approximate search of nearest neighbors)

Construct efficient multy-layered graphs to boost speed in massice volumes of data

The main idea of HNSW is to construct such a graph where a path between any pair of vertices could be traversed in a small number of steps.

All people are six or fewer social connections away from each other (six handshakes rule)

### Skip lists
Skip list is a probabilistic data structure that allows inserting and searching elements within a sorted list for O(logn) on average.

It's constructed by several layers of linked lists. The lowesr layer has all the elements. When moving to higher levels, the number of skipped elements increases (decreasing the number of connections)

![images/skip-list.jpg](images/skip_list.jpg)

