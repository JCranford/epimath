# Notes on Bayesian Epidemic Models

This document consists of my notes on the paper *A tutorial introduction to Bayesian inference for stochastic epidemic models using Markov chain Monte Carlo methods*, by Philip D. O'Neill from the School of Mathematical Sciences, University of Nottingham, published in 2002.[^full_ref]

[^full_ref]: Mathematical Biosciences 180 (2002) 103-114

These notes are not meant to be exhaustive, but rather as a stimulus to get me to focus more fully on the issues at hand. Much of the content may well be just quotations directly from the text.

## Introduction:

He begins by pointing out some of the difficulties of the analysis of epidemic data in general:

> As with any statistical modelling, thre is a balance between models that are too complicated for the data to fully inform, and those which are too simplistic to be regarded seriously as a basis for generating useful inference. In practice it is not always straightforward to achieve this balance via a formal procedure; issues of model adequacy and goodness-of-fit are not especially well-developed in the literature. Situations in which the data essentially consist of repeated independent observations (e.g. different independent outbreaks) are usually easier to assess than those featuring heavily dependent data (e.g. temporal data from a single large outbreak).[^fn2]

[^fn2]: ... and it is this latter situation that is germane to COVID.

The author discusses the differences between 'classical inference' (which assumes model parameters are fixed quantities which can be estimated from data using estimators which are random variables) and 'Bayesian inference' (which regards the model parameters as random variables and uses the 'posterior distribution - defined in Bayesian theory as the normalised product of the prior density and the likelihood - to define/calculate point and interval summaries).

He also is of the opinion that Bayesan analysis is often more straightforward in thses situations because the classical techniques because 'the usual conditions that ensure asymptotic normality of maximum likelihood estimators are often violated'.

