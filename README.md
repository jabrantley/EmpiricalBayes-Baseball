# EmpericalBayes-Baseball

These notebooks follow along with the code in the book [_Introduction to Empirical Bayes: Examples from Baseball Statistics_](https://drob.gumroad.com/l/empirical-bayes). The code in the book is written in `R` so I wanted to give it a shot in `python`. 

Here are the chapters and the corresponding notebooks. 

| Chapter    | Description                                 | File                                                   |  
| :---       | :---                                        |    :----                                               |
| Chapter 1  | Introduction                                | no notebook - no code in this chapter                  |
| Chapter 2  | The beta distribution                       | Chapter02-TheBetaDistribution.ipynb                    |
| Chapter 3  | Emperical Bayes estimation                  | Chapter03-EmpericalBayesEstimation.ipynb               |
| Chapter 4  | Credible intervals                          | Chapter04-CredibleIntervals.ipynb                      |
| Chapter 5  | Hypothesis Testing and FDR                  | Chapter05-HypothesisTestingFDR.ipynb                   |
| Chapter 6  | Bayesian A/B testing                        | Chapter06-BayesianABtesting.ipynb                      |
| Chapter 7  | Beta binomial regression                    | Chapter07-BetaBinomialRegression.ipynb                 |
| Chapter 8  | Emperical Bayesian hierarchical modeling    | Chapter08-EmpericalBayesHierarchicalModeling.ipynb     |
| Chapter 9  | Mixture models and expectation maximization | Chapter09- MixtureModels_ExpectationMaximization.ipynb |
| Chapter 10 | The multinomial and the Dirichlet           | Chapter10-MultinomialAndTheDirichlet.ipynb             |
| Chapter 11 | The ebbr package                            | no notebook - chapter just introduces R package        |
| Chapter 12 | Simulation                                  | Chapter12-Simulation.ipynb                             |
| Chapter 13 | Simulating replications                     | no notebook - see below                                |

Note: There are no notebooks for chapters 1, 11, and 13 (for now). Chapter 1 is just text and chapter 11 introduces a package that is specific to `R`. Because we are rewriting the entire project in `python`, all of the things in the `ebbr` package have already been implemented in the notebooks for chapters 2-10. There is currently no notebook for chapter 13. This chapter is simply doing replications of the simulations in chapter 12. It would be simple to add in by doing replications of the same work in chapter 12. I might work on this in the future, but for now I will probably leave it out.

Another thing to note is that the MLE solutions can be a little unstable. We need to play with the bounds and initial parameters to get a reasonable result. I found that using `pymc` can be much better, but it is also very slow. That is primarily why I did not perform the replications in Ch 13. The MLE was not giving the best paremeters but the probabilistic programming appraoch was a bit slow to perform replications without pushing the analysis onto a more powerful computing cluster for parallel operations. 

Please let me know if you find any errors or issues!
