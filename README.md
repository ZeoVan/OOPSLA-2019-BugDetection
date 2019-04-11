# The code is under reorganizing for a better structure and easier to read and understand
# Improving Bug Detection via Context-based Code Representation Learning and Attention-based Neural Networks

Bug detection has been shown to be an effective way to help developers in detecting bugs early, thus, saving
much effort and time in software development process. Recently, deep learning-based bug detection approaches
have gained successes over the traditional machine learning-based approaches, the rule-based program analysis
approaches, and mining-based approaches. However, they are still limited in detecting bugs that involve
multiple methods and suffer high rate of false positives. In this paper, we propose a combination approach of
the use of contexts and attention neural network to overcome those limitations. We propose to use as the
global context the Program Dependence Graph (PDG) and Data Flow Graph (DFG) to connect the method
under investigation with the other relevant methods that might contribute to the buggy code. The global
context is complemented by the local context extracted from the path on the AST built from the method’s
body. The use of PDG and DFG enables our model to reduce the false positive rate, while to complement
for the potential reduction in recall, we make use of the attention neural network mechanism to put more
weights on the buggy paths in the source code. That is, the paths that are similar to the buggy paths will be
ranked higher, thus, improving the recall of our model. We have conducted several experiments to evaluate
our approach on a very large dataset with +4.973M methods in 92 different project versions. The results show
that our tool can have a relative improvement up to 160% on F score when comparing with the state-of-the-art
bug detection approaches. Our tool can detect 48 true bugs in top 100 reported ones, which is 24 more true
bugs when comparing with other baselines. We also reported that our representation is better suitable for bug
detection and relatively improves over the other representations up to 206% in accuracy.
