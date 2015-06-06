---
layout: post
title: Bayesian Analysis of Traffic
header-img: "img/traffic.jpg"
---

Interestingly enough, there has been a lot of study done in the field of traffic management and the underlying patterns that are intrinsic to this system. Though none of my family members find any of this interesting, I find it particularly rewarding to explore these systems. It provides us with a problem that is different than the status quo. I did this analysis for part of my group (which consisted of [Nicholas Yager](https://nicholasyager.com/), Thomas Hartvigsen, and myself) report for the UPSTAT 2015 data competition. Since the deadline for this has passed, I feel that it is appropriate to blog about what I found.

**The Problem at Hand**

We were given data and asked to find unique patterns and provide suggestions [to better traffic conditions] for the NY Department of Transportation (NYDOT). Our data consisted of ten months of five minute measurements from a loop-detector buried 200ft from a busy intersection in Rochester, NY. In order to provide meaningful advice, I wanted to find the probability of congestion at various points in the day. This would help traffic engineers understand the relative risk of congestion so that they could take appropriate measures to mitigate these risks. In finding these probabilities, I implemented Bayes' method.

```
p(A|B) = (p(B|A)*p(A))/p(B)
```

**The Fundamental Traffic Diagram**

Essential to our understanding of how to Bayes' method, we need to be able to classify what consititutes being "congested." To do this we simply consult the fundamental traffic diagram.

![ftd]({{ site.baseurl }}/images/fundamental_traffic.png)

To understand how this relates to congestion, consult [this page](http://math.mit.edu/projects/traffic/) from MIT who provide a good explanation. For us, our Critical Density is 42.8. Anything above this number we will consider "congested," and anything below is "not congested."

**Bayesian Analysis**

```
p(C|T) = (p(T|C)*p(C))/p(T)
```

When we use the above formula (C is Congestion, T is Time) we in effect find the probability of congestion at that point in time. I simply created a matrix of these probabilities for each day and plot them as shown below.

![pCTplot]({{ site.baseurl }}/images/pCTplot.png)

Here we can see that there is a very high probability of being caught in traffic between 5:00pm and 5:30pm. When assessing the zoning in this part of Rochester there is a couple of commercial lots north of this intersection. My presumption is that this congestion is a result of individuals leaving work.
