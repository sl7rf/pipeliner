
<!-- README.md is generated from README.Rmd. Please edit that file -->
Machine Learning Pipelines for R
================================

Building machine learning models often requires pre- and post-transformation of the input and/or response variables, prior to training (or fitting) the models. For example, a model may require training on the logarithm of the response and input variables. As a consequence, fitting and then generating predictions from these models requires repeated application of transformation and inverse-transormation functions, to go from the original input to original output variables (via the model).

This package is inspired by the machine learning pipelines used in Apache Spark, and provides a common intfernace with which it is possible to:

-   define transformation and inverse-transformation functions;
-   fit a model on training data; and then,
-   generate a prediction (or model-scoring) function that automatically applies the entire pipeline of transformation and inverse-transformation to the inputs and outputs of the inner-model's predicted scores.
