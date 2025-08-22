# Internship Documentation
## Overview

This summer I worked on two projects that helped me build skills in Python, data handling, and applied machine learning. The first was an Email Spam Classifier, which introduced me to the full workflow of training and testing models. The second was an AI Hallucination Detection system, a more exploratory project focused on identifying when large language models produce inaccurate but confident-sounding responses.

Both projects came with their own challenges, which pushed me to problem-solve and develop a deeper understanding of how AI systems are built and maintained.

## Project 1: Email Spam Classifier

### Goal:
Train a model to classify email messages as either spam or not spam.

### What I Did:

* Preprocessed text data and extracted numerical features.

* Split data into training and testing sets.

* Trained the model using model.fit(X_train_features, Y_train).

* Focused on completing the entire machine learning pipeline, even with a basic implementation.

### Challenges:

* Limited understanding of how to adjust which features the model learned from.

* Needed to figure out how to experiment with different training inputs and parameters.

### Outcome:

* Built a functional spam classifier.

* Gained a working knowledge of model training workflows.

* Established a foundation that made it easier to take on more complex projects.

# Project 2: AI Hallucination Detection

Goal: 

Develop a proof of concept system to detect when an AI model is “hallucinating” (generating answers that sound correct but are inaccurate) and gives a confidence score from 0-100 how cofident the output is and gives an assessment.

What I Did:

Cleaned and formatted training data.

Applied tokenization and padding so models could process text consistently.

Experimented with different modeling approaches to score responses on a 0–100 reliability scale.

Ran error analysis and built simple visualizations to track performance.

Challenges and Solutions:

Model downloads failing (SSL error): Hugging Face wouldn’t download models due to SSL issues. I solved this by downloading models locally and pointing my code to the local path.

Deprecation warnings and unused weights: Learned how to update code to match changes in the Transformers library.

Data handling mistakes: Accidentally wiped dictionaries, which taught me how Python manages objects and references.

Defining hallucinations: Learned that the concept isn’t always black and white, and adapted scoring methods to account for this ambiguity.

Outcome:

Built a working prototype capable of testing multiple models and comparing results.

Created basic graphs to visualize error patterns.

Documented the workflow to track progress and share learnings.

Key Takeaways

Learned the end-to-end workflow of training and testing models, from data prep to evaluation.

Developed stronger debugging skills, especially when facing library issues and system errors.

Learned how to adapt and problem-solve when things didn’t work as expected (like the SSL error with Hugging Face).

Built confidence in tackling open-ended AI problems that don’t always have clear solut
