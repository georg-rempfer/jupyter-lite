# What is this?

This is a collection of interactive statistics calculations commonly used to evaluate test results. They aim at quantifying the information about the performance of a system under test that can be deduced from your test results.

# What evaluations are implemented?

Among the notebooks, you will find frequentist and Bayesian evaluations for the relevant unknown experimental parameters (success probability for discrete tests, event occurrence rate for continuous tests), plots of the outcome distributions when all parameters are known, and evaluations that let you compare the results from multiple different tests.

With the calculations provided here, you could, for example, answer the following questions:

### The subdirectory `bernoulli_process` contains evaluations for discrete tests with success/failure results.

[bernoulli_process/binomial_distribution.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Fbinomial_distribution.ipynb) *- "I have a system which does its job correctly 96% of the time. If I run it 200 times, how many successful runs and how many failures can I expect with which probability?"*

[bernoulli_process/frequentist_confidence.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Ffrequentist_confidence.ipynb) *- "I have run a test with 200 repetitions, got 184 successes and 16 failures. How sure can I be that my system's success rate is higher than 90%? I want a conservative estimate."*

[bernoulli_process/frequentist_confidence_interval.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Ffrequentist_confidence_interval.ipynb) *- "I have run a test with 200 repetitions, got 184 successes and 16 failures. What success rate can I promise with 95% confidence? I want a conservative estimate."*

[bernoulli_process/bayesian_posterior.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Fbayesian_posterior.ipynb) *- "I have run a test with 200 repetitions, got 184 successes and 16 failures. What does this tell me about the different success rates the system might possess? I don't want conservative estimates, I want best guesses and maybe even add in some prior expectation."*

[bernoulli_process/bayesian_credibility.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Fbayesian_credibility.ipynb) *- "I have run a test with 200 repetitions, got 184 successes and 16 failures. How sure can I be that my system's success rate is higher than 90%? I don't want a conservative estimate, I want a best guess and maybe even add in some prior expectation."*

[bernoulli_process/bayesian_credible_interval.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Fbayesian_credible_interval.ipynb) *- "I have run a test with 200 repetitions, got 184 successes and 16 failures. What success rate can I promise with 95% confidence? I don't want a conservative estimate, I want a best guess and maybe even add in some prior expectation."*

[bernoulli_process/bayesian_pair_credibility.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Fbayesian_pair_credibility.ipynb) *- "I previously tested my system 100 times, got 92 successes and 8 failures. Recently, someone else conducted 10 tests of which 8 were successful and 2 failed. I think they just had bad luck, but they claim there is some new problem. How much belief should I put into either possibility? How many more tests do we have to do to be sure?"*

[bernoulli_process/bayesian_two_stage_testing.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=bernoulli_process%2Fbayesian_two_stage_testing.ipynb) *-"Soon someone else will test my system 10 times and I want to know what they will probably see. I don't know my systems success probability exactly but i have previously tested it 20 times, got 17 successes and 3 failures. I don't want a conservative estimate, I want a best guess and maybe even add in some prior expectation."*

### The subdirectory `poisson_process` contains evaluations for continuous tests during which discrete events occur.

[poisson_process/poisson_distribution.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Fpoisson_distribution.ipynb) *- "I have a system which produces a failure every 100 hours. If I run it for 200 hours, how many failures can I expect with which probability?"*

[poisson_process/frequentist_confidence.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Ffrequentist_confidence.ipynb) *- "I have run a test for 50 hours and got 4 failures. How sure can I be that my system's failure rate is lower than 1 failure / 10 hours? I want a conservative estimate."*

[poisson_process/frequentist_confidence_interval.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Ffrequentist_confidence_interval.ipynb) *- "I have run a test for 50 hours and got 4 failures. What failure rate can I promise with 95% confidence? I want a conservative estimate."*

[poisson_process/bayesian_posterior.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Fbayesian_posterior.ipynb) *- "I have run a test for 50 hours and got 4 failures. What does this tell me about the different failure rates the system might possess? I don't want conservative estimates, I want best guesses and maybe even add in some prior expectation."*

[poisson_process/bayesian_credibility.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Fbayesian_credibility.ipynb) *- "I have run a test for 50 hours and got 4 failures. How sure can I be that my system's failure rate is lower than 1 failure / 10 hours? I don't want a conservative estimate, I want a best guess and maybe even add in some prior expectation."*

[poisson_process/bayesian_credible_interval.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Fbayesian_credible_interval.ipynb) *- "I have run a test for 50 hours and got 4 failures. What failure rate can I promise with 95% confidence? I don't want a conservative estimate, I want a best guess and maybe even add in some prior expectation."*

[poisson_process/bayesian_pair_credibility.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Fbayesian_pair_credibility.ipynb) *- "I previously tested my system for 100 hours and got 12 failures. Recently, someone else ran it for 10 hours and got 2 failures. I think they just had bad luck, but they claim there is some new problem. How much belief should I put into either possibility? How much longer do we have to do to be sure?"*

[poisson_process/bayesian_two_stage_testing.ipynb](https://georg-rempfer.github.io/jupyter-lite/lab/index.html?path=poisson_process%2Fbayesian_two_stage_testing.ipynb) *-"Soon someone else will test my system for 10 hours I want to know how many failures they will probably see. I don't know my systems failure rate exactly but i have previously tested it for 20 hours, and got 3 failures. I don't want a conservative estimate, I want a best guess and maybe even add in some prior expectation."*

# FAQ

### Can I trust the results?

We cannot guarantee that the calculations in the default notebooks are correct. You need to do your own validation.

### Where are the notebooks stored?

Default notebooks are stored on server. If you make changes to those or create your own notebooks from scratch, these are stored in your browser cache. They will only be visible to you on the machine you are using when you create them. You are responsible to create your own backups (download by right clicking in the browse side pane, upload button at the top of the browse side pane).

### How do I get back the default notebook after making changes?

You can delete notebooks that are available by default to return them to their original state. If you want to return the whole application to the latest default state (and lose all your changes and custom notebooks), you can delete the browser cache for this website and refresh.

### How are the computations performed?

All computations are run on your machine in the browser. These notebooks use the Pyodide Python kernel - a webassembly implementation of the Python interpreter and all used packages. If you plan to run more elaborate calculations, other environments are more suitable.

### I want to fix a mistake in one of the default notebooks or contribute my own evaluations!

You can do so here: https://github.com/georg-rempfer/jupyter-lite