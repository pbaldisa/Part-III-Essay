# Points of infinite multiplicity of planar Brownian motion

Despite its simple definition, Brownian motion exhibits a very rich structure, often hiding remarkable and unintuitive properties. Its first mathematical construction is due to Norbert Wiener in 1923, 
but it owes its name to Robert Brown, who observed the erratic motion of pollen particles in water in 1827. Other early works in Brownian motion include the physical model developed by Einstein, 
and Bachelier's thesis on pricing stock options, both in the early 1900s. Paul Lévy also contributed greatly to the theory of Brownian motion with his monograph in 1958.

The main objective of this essay is not to present original results, but to explore a mathematically rich and subtle topic within probability and convey it in an accessible way. 
The intended audience consists of students in Mathematics who are comfortable with probability and measure theory at the level of the Part III course in Advanced Probability. 
In particular, familiarity with the basic theory of Brownian motion is assumed.

Brownian motion exhibits different behaviour depending on the ambient dimension. Some of its better known properties are recurrence and transience. Linear Brownian motion is point recurrent, 
meaning that the set of hitting times for any point is unbounded almost surely. Planar Brownian motion, on the other hand, is point transient, i.e. it does not hit points. However, it is 
neighbourhood recurrent, meaning that, with probability one, it returns to a ball around any given point infinitely often. This and the title of the essay raise an intriguing question: if 
planar Brownian motion does not hit points, in what sense can it have multiple points? We address this question by showing that, despite not hitting any individual point, it nonetheless intersects itself 
in such a way that certain locations are visited infinitely many times.

This essay aims to explore some machinery that makes this result precise and provable. The fundamental tools are the intersection local times, presented in **2.Local times**. These are measures that 
offer a rigorous way to quantify the time Brownian paths spend intersecting each other. Their construction is technically involved and may seem opaque at first, but we will see how these objects offer 
deep insight into the structure of Brownian motion. Most results and ideas in this section are from Le Gall's book _Some properties of planar Brownian motion_ and _Random walk intersections : 
large deviations and related topics_ by  Chen. Before continuing, we end this part with a mention of local times for one dimensional Brownian motion, which are the original object that motivates their name, 
and was first studied by Lévy.

In the second half of the essay, in **3.Multiple points**, we study the occurrence and nature of points that are revisited by the Brownian path. This includes points of infinite multiplicity that give name 
to this essay, but also finite multiple points. To build intuition, we examine, in particular, double points. In this brief overview, we introduce the concept of renormalisation, which is much richer and 
hard to approach in general, but it is insightful in the case of double points. At this stage, our focus is to introduce the final tools necessary, and culminate all our previous efforts with a proof of 
almost sure existence of multiple points. This not only establishes the presence of such points, but also provides a characterisation of the structure of the set of times at which the Brownian path visits 
such points, which is in itself a testament to the richness and complexity of Brownian motion. The primary ideas here come from Le Gall in _Some properties of Brownian motion_ and _Le comportement du mouvement 
brownien entre les deux instants où il passe par un point double_.

As a historical note, the study of intersection local times and multiple points in Brownian motion has deep roots in both probability theory and mathematical physics. 
The concept of intersection local time was initially motivated by physical models, with foundational contributions by Edwards, Symanzik, Varadhan, and Wolpert. Geman, Horowitz, and Rosen 
exploited the Gaussian nature of Brownian motion to obtain precise results. In parallel, the question of points of finite or infinite multiplicity in Brownian paths was settled through the work of Dvoretzky, 
Erdős, Kakutani, and Taylor. Although their proof of points of infinite multiplicity for planar Brownian motion was not complete. Le Gall introduced a new proof, which is presented here. 
These two topics — intersection local times and multiple points — form the core of this essay.
