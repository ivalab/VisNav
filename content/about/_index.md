+++
title = "IVALab Vision-Based Navigation Research"
+++

Our research is inspired by earlier work on _controlled active vision_,
which examines the role of visual sensors in the feedback loop and
investigates how to design visual algorithms whose closed-loop
performance can be made to reproduce the properties of ideal feedback
control laws (in terms of their frequency domain responses or in
terms of some other established performance scoring function). 
Importantly, it also looks at the role that online estimation and
adaptation plays in ensuring that the visual algorithm is operating
within the correct domain of attraction regarding its internal state
model.  Vision is an interesting modality because some processing must
occur in order to arrive at the feedback signal of interest. That
processing itself impacts the operation of the closed-loop system, so it
must be designed and managed to optimize performance.  Finally, 
we take into consideration the real-time demands of the visual
algorithm. Doing so requires balancing numerical methods and algorithmic
implementation against solution complexity.  High performance is
meaningless if the algorithm cannot be implemented in real-time.

Here, we focus this perspective on the problem of collision-free
navigation through an unknown and uncontrolled space.  Most traditional
pipelines live at two extremes. On one side, there is sufficient
computational performance so that the idealized perceive, plan, act
approach can be realized. On the other side, more advanced data structures
and sensor throughput restrictions permit compute limited platforms to
achieve real-time computations. Issues arrive when looking at the
spectrum of computation, sensor throughput, and task complexity.
Algorithms designed for high performance machines do not scale down to
low performance computers.  Algorithms designed to optimize sensory data
access do not scale up to higher sensor throughputs. Our aim is to
establish a navigation algorithm with deterministic properties that can
be tuned based on the platform characteristics, or whose abilities can
be predicted based on the platform characteristics.

At the heart of this lies a _perception-space_ approach to computation.
Rather than employ optimized but poorly-scaled data structures, and
rather than brute force the conversion of the data into a globally
consistent reference frame, we advocate for minimally processing the
sensory data and mapping the collision-avoidance problem from a spatial,
world representation to a visual, perceptual representation.  Don't map
the data to the robot's physical domain, but map the physical robot into
the sensor's egocentric domain. We call this egocentric approach
_Planning in Perception Space_ or _PiPS_, and have just begun to
explore the benefits of such an intermediate representation for
generating computationally scalable navigation algorithms. Longer term,
we aim to also explore how these local methods can more robustly
integrate with global methods and exploit the multiple time-scales that
the different modules should operate at with regards to data
assimilation, solution rate, and other high-level navigation
meta-decisions.



### Investigators Involved

- [Patricio A. Vela](http://pvela.gatech.edu)
- Justin S. Smith (graduate)
- Shiyu Feng (graduate)
- Fanzhe Lyu (undergraduate)
- Ruoyang Xu (undergraduate)

### Former Investigators

- Jin Ha Hwang
