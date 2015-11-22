# Bayesian statistics
## Syllabus 

1. The Baysian formula: 
	
	$Pr(\theta|data) = \frac{Pr(data|\theta)Pr(\theta)}{Pr(data)}$
	
	The aim is to derive the posterior (LHS), a probability density for all the possible values of $\theta$. In the numerator we have the likelihood (sort of a probability for ending up with the observed data given our selection for $\theta$). Also we have the prior, which represents the pre-experimental knowledge of the parameter values. For example, we might assume that the probability of all the possible values of $\theta$ are equally likely, i.e. use a uniform distribution.
	
	The denominator normally turns out to be the most difficult to work out. It tells us the probability of the data over all possible choices of $\theta$.

1. Start with assumption that prior and posterior are conjugate. This makes things easy in that it gives us a closed form for the posterior.
1. Move on to the more complex situation when we do not have a conjugate prior. This leads us to a computational approach. Options include: Grid approximation, Metropolis Hastings algorithm (uses sampling), Gibbs sampling (BUGS).
1. How linear and GLMs can make use of Bayesian statisitics. 
1. Hierarchical models - placing a prior on prior parameters.
1. Simulation methods
1. Bayesian decision theory - (associate costs with wrong decision).

## Bayes vs Frequentist Probabilities

What is the probability of getting a head in a flip of a coin...

### Frequentist

Probability of a head is represented by the relative frequency of getting a head in a long series of identical flips.

*Data vary, parameters fixed.*

One problem is what do we mean by 'identical'?

Another problem arises where we can't imagine an infinite number of identical experiments e.g. an infinite number of football games between F and E to determine the probability that E wins.

### Bayesian

Probability of a head is equal to the number of heads divided by the number of possibilities. 

*Data is fixed. Parameters vary.* 

The probability represents the uncertainty where the uncertainty creeps in due to the fact that we do not know the initial conditions exactly. The probability of a head has a PDF. Note - the Bayes view does not rely on a long run frequency of flips.

For the football example, again the probability is the uncertainty as to whether E will win. This can be construed as a subjective view.


## Marginal Probability

Two random variables, $X$ disease status (1 if subject actually has disease) and $Y$ symptoms for the disease (1 if individual is symptomatic of the disease). 

[id]:fig1.jpg































