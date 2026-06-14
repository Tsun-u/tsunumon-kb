# Theme A4: Machine Learning

> New IB Computer Science syllabus (first teaching 2025, first assessment 2027) — Theme A "Concepts of Computer Science".
> A4.1 and A4.4 are **SL + HL**. A4.2 (Data preprocessing) and A4.3 (Machine learning approaches) are **HL only**.
> Depth: students must **understand the principles and ethical implications** of machine learning. The syllabus does **not** require mathematical derivation (e.g. deriving back-propagation) or hands-on implementation of models.

## A4.1 Machine Learning Fundamentals (SL + HL)

### What machine learning is
- **Machine learning (ML)** is a branch of artificial intelligence where a system **learns patterns from data** rather than following explicitly programmed rules.
- In traditional programming, a human writes the logic; in ML, the system **infers the rules** from examples (data + expected outputs → a model).
- A **model** is the learned function that maps inputs to outputs after training.

### Categories of learning
| Type | What it learns from | Goal | Example |
|------|--------------------|------|---------|
| **Supervised learning** | Labelled data (inputs paired with correct outputs) | Predict the label for new inputs | Spam detection, image classification, house-price prediction |
| **Unsupervised learning** | Unlabelled data | Find structure/groupings in the data | Customer segmentation (clustering), anomaly detection |
| **Reinforcement learning** | Feedback (rewards/penalties) from an environment | Learn a policy that maximises cumulative reward | Game-playing agents, robot navigation |

- **Classification** vs **regression** (both supervised): classification predicts a *category* (discrete); regression predicts a *continuous value*.
- **Clustering** is the typical unsupervised task: grouping similar items without predefined labels.

### The training process (conceptual)
- Data is split into a **training set**, a **validation set**, and a **test set**.
- The model adjusts its internal **parameters (weights)** to reduce the error on the training data, measured by a **loss function** (also called cost/error).
- **Generalisation** is the goal: performing well on *unseen* data, not just memorising the training set.
- **Overfitting**: the model fits the training data too closely (including noise) and performs poorly on new data.
- **Underfitting**: the model is too simple to capture the underlying pattern, so it performs poorly even on training data.

## A4.2 Data Preprocessing (HL only)

Raw data almost never arrives in a form ready for training. Preprocessing transforms it into something a model can learn from effectively.
- **Data cleaning**: handling missing values, removing duplicates, correcting errors, dealing with outliers.
- **Normalisation / scaling**: rescaling numeric features to a common range (e.g. 0–1) so that no single feature dominates due to its units.
- **Encoding**: converting categorical values into numeric form (e.g. one-hot encoding).
- **Feature selection / feature engineering**: choosing or constructing the most informative inputs; removing irrelevant or redundant features to improve accuracy and reduce training cost.
- **Data splitting**: partitioning into training/validation/test sets so performance is measured honestly.
- **Why it matters**: model quality is bounded by data quality. Biased or unrepresentative training data produces biased models (links to A4.4).

## A4.3 Machine Learning Approaches (HL only)

### Artificial Neural Networks (ANN)
- An **artificial neural network** is a computational model loosely inspired by biological neurons, built from interconnected **nodes (neurons)** organised in **layers**.
- It learns to model **complex, non-linear patterns** by adjusting connection **weights** during training.

#### The perceptron (single neuron)
- A **perceptron** is the simplest neural unit. It:
  1. takes several **inputs**, each multiplied by a **weight**,
  2. sums them and adds a **bias**,
  3. passes the result through an **activation function** to produce an output.
- A single perceptron can only separate data that is **linearly separable** (it draws one straight boundary). This is its key limitation.

#### Multi-Layer Perceptron (MLP)
- An **MLP** stacks neurons into layers:
  - **Input layer** — receives the feature values.
  - **Hidden layer(s)** — intermediate layers where non-linear combinations are learned.
  - **Output layer** — produces the final prediction.
- With one or more hidden layers and non-linear activations, an MLP can model patterns a single perceptron cannot (e.g. the classic XOR problem).
- **Deep learning** = neural networks with **many hidden layers** ("deep" networks), able to learn hierarchical features from large datasets.

#### How a network learns (conceptual only)
- **Forward pass**: inputs flow through the layers to produce a prediction.
- A **loss function** measures how wrong the prediction is.
- **Gradient descent**: weights are nudged in the direction that **reduces the loss**, step by step. The step size is the **learning rate**.
- **Back-propagation**: the mechanism that distributes the error backwards through the layers to update each weight.
- IB depth note: students should grasp this **intuition** (a network repeatedly adjusts weights to reduce error); the **maths is not examined**.

#### Convolutional Neural Networks (CNN)
- A **CNN** is a neural network specialised for **grid-like data, especially images**.
- **Convolutional layers** apply filters that detect local features (edges, textures), and stacking them lets the network learn a **hierarchy of spatial features** (edges → shapes → objects).
- Typical use: image classification and recognition.

### Other approaches
- **Genetic algorithms**: optimisation inspired by **natural selection** — a population of candidate solutions evolves through **selection, crossover, and mutation**, keeping the fittest candidates across generations.
- **Reinforcement learning**: an **agent** takes **actions** in an **environment** and receives **rewards**; over time it learns a **policy** that maximises long-term reward. Key ideas: state, action, reward, exploration vs exploitation.

## A4.4 Ethical Considerations (SL + HL)

- **Bias**: when training data over- or under-represents certain groups, the model's outputs become systematically skewed. ML can reproduce and amplify the biases present in the data it was trained on.
- **Fairness**: a model should not produce outcomes that systematically disadvantage people on the basis of protected characteristics such as race or gender.
- **Transparency / explainability**: many models, particularly deep networks, function as **"black boxes"** — it is difficult to explain *why* a particular decision was reached. This raises serious concerns in high-stakes contexts like lending, hiring, healthcare, and the justice system.
- **Accountability**: when an automated decision causes harm, the question of who bears responsibility — developer, deployer, or user — is unresolved.
- **Privacy**: training ML systems typically demands large volumes of personal data, raising questions about consent and how that data is stored and used.
- **Societal impact**: workforce displacement from automation, the spread of AI-generated misinformation, and the significant energy costs of training large models are all active concerns.

## Modern Applications: LLMs and RAG

> Not a formal IB sub-topic, but included because teaching/assessment questions increasingly cover these and they build directly on the neural-network concepts above.

- **Large Language Models (LLMs)** are very large neural networks (transformer architecture) trained on huge text corpora to predict the next token. They power chatbots and text generation.
- **Hallucination**: an LLM can produce fluent but **factually wrong** output, because it predicts plausible text rather than retrieving verified facts.
- **Retrieval-Augmented Generation (RAG)**: a technique that **retrieves relevant documents** from an external knowledge source and feeds them to the model as context, so answers are **grounded in real data** instead of relying only on the model's parameters. RAG reduces hallucination and lets a model use up-to-date or private information without retraining.
- Pipeline of RAG (conceptual): **query → retrieve relevant documents → augment the prompt with them → generate a grounded answer**.

## Key Terminology

| Term | Definition |
|------|-----------|
| **Machine learning** | A category of AI where systems improve their performance by learning from data rather than from hand-coded rules |
| **Model** | The learned input→output function produced by training |
| **Supervised learning** | Learning from labelled examples to predict labels for new inputs |
| **Unsupervised learning** | Finding structure (e.g. clusters) in unlabelled data |
| **Reinforcement learning** | An agent learns a policy by maximising reward from an environment |
| **Training / test set** | Data used to fit the model vs. held-out data used to measure generalisation |
| **Loss function** | A measure of the gap between the model's predictions and the correct answers |
| **Overfitting** | A model that memorises training data too closely, capturing noise, and then fails to generalize to new examples |
| **Perceptron** | A single artificial neuron: weighted sum + bias → activation function |
| **Weight / bias** | Learnable parameters scaling inputs / shifting the activation |
| **Activation function** | Non-linear function applied to a neuron's output, enabling complex patterns |
| **MLP** | Multi-layer perceptron: input, hidden, and output layers |
| **Hidden layer** | Intermediate layer where non-linear feature combinations are learned |
| **Deep learning** | Neural networks with many hidden layers |
| **Gradient descent** | Iteratively adjusting weights to reduce the loss |
| **Back-propagation** | Propagating error backwards to update each weight |
| **CNN** | Convolutional neural network; learns hierarchical spatial features, used for images |
| **Genetic algorithm** | An optimisation technique that mimics evolution — a population of solutions competes, combines, and mutates across generations |
| **Bias (ethical)** | Systematic unfairness in a model's predictions caused by imbalanced or skewed training data |
| **Black box** | A model whose internal decision process cannot be easily inspected or explained |
| **LLM** | Large Language Model; a large neural network for text generation |
| **RAG** | Retrieval-Augmented Generation; grounds model output in retrieved documents |

## Common Misconceptions

1. **"Machine learning is just normal programming."** — In traditional programming a human writes the rules; in ML the rules (the model) are *learned from data*.
2. **"A single perceptron can solve any problem."** — A single perceptron only handles **linearly separable** data; you need hidden layers (an MLP) for problems like XOR.
3. **"More layers / more data is always better."** — Larger models can **overfit**, cost more to train, and need more data; the right size depends on the problem.
4. **"Neural networks think like a human brain."** — They are *loosely inspired* by neurons but are mathematical functions optimised on data, not conscious reasoning.
5. **"AI is objective because it's a machine."** — Models inherit the **biases** embedded in their training data; no dataset is truly neutral.
6. **"An LLM knows facts."** — An LLM predicts statistically likely text sequences and can **hallucinate**; grounding it (e.g. with RAG) is what makes answers more reliable.
7. **"Supervised and unsupervised learning are the same."** — Supervised learning requires **labelled** data; unsupervised learning works on **unlabelled** data.

## Comparison with AP Computer Science

- **AP CS A** is purely Java programming and OOP — it contains **no machine learning** content.
- **AP CS Principles** touches AI only at the level of **computing bias / ethics** and responsible use of generative-AI tools; it has **no neural-network technical content**.
- IB CS (2027) is the only one of the three with explicit **ML/neural-network theory** as core/HL content — making this file the primary reference for any neural-network teaching question.
