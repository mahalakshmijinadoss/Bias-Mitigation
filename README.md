# Bias-Mitigation

Repository for Course Project Bias Mitigation

Our first baseline model uses a pre-trained BERT model and two linear layers. Our second baseline model has an embedding layer, a bidirectional LSTM encoder, an attention mechanism, and one linear layer.

We Implement 2 Architectures:
The classifier uses a pre-trained BERT model followed by two linear layers for toxicity prediction, and the adversary has two linear layers. Both models are pre-trained for three epochs. They are then adversarially trained over 30 iterations, where the adversary learns to predict a protected attribute from the classifier’s output.

The second debiasing architecture uses a BiLSTM encoder with attention, a classifier for the target label, and an adversary for the protected attribute. After pretraining the encoder and classifier, adversarial training alternates between training the adversary and updating the encoder to confuse it. The objective is to retain task-relevant information while minimizing leakage of protected attributes.










