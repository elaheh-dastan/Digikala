One common form of embedding-based IR application is dense retrieval, where relevant answers to the query can be retrieved based on the embedding similarity.

Multi-vector retrieval where the fine-grained relevance between query and document is computed based on the interaction score of multiple embeddings.

Sparse or lexical retrieval where the importance of each term is estimated by its output embedding.

M3-Embedding is pronounced for its breakthrough of versatility in working languages, retrieval functionalities, and input granularities.

By learning a common semantic space for different languages, enables both multilingual retrieval within each language and crosslingual retrieval between different languages.

Self-Knowledge Distillation (Self-KD) is a model training technique where a neural network is trained using its own predictions as "soft targets" in addition to the ground truth labels. The goal is to improve generalization, robustness, and performance by refining the model’s own knowledge. 

Self-KD is based on the concept of Knowledge Distillation (KD), where a smaller "student" model learns from a larger "teacher" model. However, in Self-KD, the same model acts as both the teacher and the student.

1. Teacher Predictions: During training, the model produces both:
    Hard Labels (from the dataset)
    Soft Labels (logits from an earlier version of the model or different layers)

2. Loss Function: The total loss combines:
    Standard Loss (Cross-Entropy Loss): Encourages learning from true labels.
    Distillation Loss (KL-Divergence Loss): Encourages the model to match its own earlier predictions (soft labels).

3. Training Strategy: There are different ways to implement Self-KD:
    Same Model, Different Epochs: Earlier predictions from the model serve as soft labels in later epochs.
    Layer-wise Distillation: Deeper layers learn from earlier layers in the same model.
    Augmented Views: The model is trained on different augmentations of the same input and distills knowledge across them.

Benefits:
    Improves Generalization: Helps the model avoid overfitting by smoothing decision boundaries.
    Enhances Robustness: Reduces sensitivity to noise in labels.
    No Need for a Separate Teacher Model: Saves computational cost compared to traditional KD.
    Better Representation Learning: Encourages consistency in model predictions.

Based on the principle of ensemble learning, such heterogenous predictors can be combined as a stronger predictor. Thus, we integrate the relevance scores from different retrieval functions as the teacher signal, which is used to enhance the learning process via knowledge distillation.

We optimize the batching strategy to achieve a large batch size and high training throughput, which substantially contributes to the discriminativeness of embeddings.
