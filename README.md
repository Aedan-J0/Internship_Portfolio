# Internship Documentation
## Overview

This summer I worked on two projects that strengthened my skills in Python, data handling, and applied machine learning. The first was an Email Spam Classifier, which gave me a foundation in the full workflow of training and testing models. The second was an AI Hallucination Detection prototype, a more exploratory project focused on identifying when large language models produce inaccurate but confident-sounding responses.

Both projects were functional at a proof-of-concept level. The focus was on learning workflows, troubleshooting problems, and exploring approaches that could be expanded with more time.

## Project 1: Email Spam Classifier

### Goal:

Train a model to classify email messages as either spam or not spam.

### What I Did:

* Preprocessed text data and extracted numerical features.

* Split data into training and testing sets.

* Trained the model using model.fit(X_train_features, Y_train).

* Focused on completing the machine learning pipeline, even with a basic setup.

### Challenges:

* Limited understanding of how to adjust which features the model learned from.

* Needed to figure out how to experiment with different training inputs and parameters.

### Outcome:

* Built a functional spam classifier.

* Learned the end-to-end workflow of training/testing models.

* Created a foundation that made it easier to take on more complex projects.

## Project 2: AI Hallucination Detection

### Goal:

Develop a proof of concept system to detect when an AI model is “hallucinating” (generating answers that sound correct but are inaccurate) as well as gives a confidence score of 0-100 regaring how confident the LLM's output is. It also gives an asessment on it.

### What I Did:

* Cleaned and formatted training data.

* Applied tokenization and padding so models could process text consistently.

* Experimented with different modeling approaches to score responses on a 0–100 reliability scale.

* Ran error analysis and built visualizations to track performance.

### Challenges and Solutions:

 * Hugging Face SSL Error: Models would not download due to SSL issues. I solved this by downloading models locally and pointing the code to the local path.

* Deprecation warnings and unused weights: Learned how to update code to match library changes.

* Data handling mistakes: Accidentally wiped dictionaries, which helped me understand how Python manages objects and references.

* Defining hallucinations: Learned that “wrong” isn’t always clear-cut, so evaluation had to be flexible.

### Outcome:

* Built a working prototype capable of testing multiple models and comparing results.

* Created graphs to visualize error patterns.

* Documented the workflow to keep track of progress and share learnings.

## Reflection
### What Actually Came to Fruition

* A working Email Spam Classifier that completed the full ML workflow.

* A Hallucination Detection prototype that could score model responses and generate visualizations.

### What Impediments Did I Face?

* SSL errors preventing Hugging Face model downloads.

* Frequent deprecation warnings and version issues in Transformers.

* Data handling mistakes in Python (especially with dictionaries).

### What Was Easy to Grasp?

* The spam classifier workflow (preprocessing, training, testing).

* Tokenization and padding once I saw how models required consistent inputs.

* Visualization with charts and graphs to make model results easier to understand.

### With Additional Time, Where Would I Like to See This Go?

* Spam Classifier: Experiment with different feature extraction methods and hyperparameters to improve accuracy.

* Hallucination Detector:

  * Expand dataset with more examples.

  * Explore advanced model architectures and ensembles.

  * Build a clearer, benchmarked scoring system.

  * Turn results into a simple interactive dashboard.

  * Implement cosine similarity to take a user’s question, compare it against a dictionary of pre-written question–answer pairs, and automatically return the closest match. This would make the system more practical by bridging free-form input with structured responses.

## Key Takeaways

- Gained experience with the end-to-end machine learning workflow, from preprocessing to evaluation.

- Improved at debugging and adapting when libraries broke or systems failed.

- Learned to problem-solve creatively, like bypassing SSL errors by switching to local models.

- Developed more confidence tackling open-ended AI problems with no single “right” solution.
