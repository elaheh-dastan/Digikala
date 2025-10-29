# ACID vs BASE
ACID databases prioritize consistency over availability—the whole transaction fails if an error occurs in any step within the transaction. 
In contrast, BASE databases prioritize availability over consistency. Instead of failing the transaction, users can access inconsistent data temporarily. 
Data consistency is achieved, but not immediately.

Modern databases are distributed data stores that replicate data across multiple nodes connected by a network. They allow users to perform multiple data manipulations like reads and writes in a single transaction. Users expect data to remain consistent across all nodes at the end of the transaction. However, in theoretical computer science, Brewer's theorem (also called CAP theorem) states that any distributed data store can provide only two of the following three guarantees:

Consistency: every read operation receives the most recently updated data or an error.

Availability: every database request receives a successful response, without guaranteeing it contains the most recently updated data.

Partition tolerance: the system continues to operate despite dropped or delayed messages between the distributed nodes

# ACID 
ACID stands for atomicity, consistency, isolation, and durability.

Isolation ensures that a new transaction, accessing a particular record, waits until the previous transaction finishes before it commences operation.

Durability ensures that the database maintains all committed records, even if the system experiences failure. It guarantees that when ACID transactions are committed, 
all changes are permanent and unimpacted by subsequent system failures. For example, in a messaging application, when a user sends a message and receives a confirmation of successful delivery, 
the durability property ensures that the message is never lost. This remains true even if the application or server encounters a failure.
