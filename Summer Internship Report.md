Summer Internship Report
What Actually Came to Fruition

Two main projects reached working stages:

Email Spam Classifier – I built and trained a model that could distinguish between spam and non-spam emails. While basic, it gave me experience with preprocessing, feature extraction, training, and testing, completing a full machine learning workflow.

AI Hallucination Detection Prototype – I developed a proof-of-concept system that tested different models to see when they produced inaccurate but confident responses. I was able to clean and prepare data, tokenize text, run models locally, and generate basic visualizations to compare results.

Both projects were functional but intentionally left at an experimental stage. The focus was on learning workflows and testing approaches, not on building polished production systems.

What Impediments Did You Face?

Hugging Face SSL Errors: Models wouldn’t download, blocking progress. I solved this by downloading them locally and pointing the code to those files.

Deprecation Warnings: Transformers library updates broke some of my initial code, which forced me to learn how to adapt to changing APIs.

Data Handling Mistakes: At one point I wiped entire dictionaries by accident, which taught me more about how Python handles objects.

Defining “Hallucinations”: Figuring out what counts as a “wrong” answer wasn’t always clear, making evaluation more subjective than expected.

What Was Easy to Grasp?

The Spam Classifier Workflow: Once I understood how to preprocess data and run model.fit, the full cycle of training/testing was straightforward.

Tokenization Concepts: Breaking down text into tokens and padding them felt logical once I saw how models rely on consistent input sizes.

Visualization: Building simple graphs to compare performance was quick and made the results more tangible.

With Additional Time, Where Would I Like to See This Go?

For the Spam Classifier, I would have experimented with different feature extraction methods and hyperparameters to improve accuracy beyond the baseline.

For the Hallucination Detector, I would have:

Expanded the dataset with more examples of both accurate and hallucinated responses.

Tried more advanced model architectures and ensemble approaches.

Built a clearer scoring system with benchmarks to measure trustworthiness more consistently.

Improved the visualizations into a small dashboard that could showcase patterns in real time.

With more time, both projects could evolve into tools that are not just prototypes, but also practical resources for analyzing and improving AI reliability.
