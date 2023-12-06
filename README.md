# Graph_NN
Practice files for understanding GNNs
In the context of graph neural networks (GNNs), a graph is typically represented by nodes (vertices) and edges connecting these nodes. Each node in the graph can have associated features or attributes, which are often represented as a feature vector. These node features capture information about the characteristics or properties of each node in the graph.

For example, in a social network graph, each node might represent a user, and the associated node features could include attributes such as age, gender, and the number of friends. In a citation network, nodes might represent academic papers, and the node features could include information about the content of the papers, publication year, and author information.

When we talk about "node features" in the context of GNNs, we are referring to these attribute vectors associated with each node in the graph. These features serve as input to the GNN model, and the model processes this information to make predictions or perform tasks on the graph.

Global mean pooling is a technique used to aggregate information from all nodes in the graph. Specifically, it calculates the mean (average) of the node features across all nodes. This aggregated feature vector represents a summary or global view of the entire graph. In the provided code, after applying the graph convolutional layers (conv1, conv2, conv3), the global mean pooling operation (global_mean_pool) is used to aggregate the node features across the entire graph, resulting in a single feature vector for each graph in the batch. This aggregated vector is then further processed by the final classifier (lin) to make predictions for the entire graph.
