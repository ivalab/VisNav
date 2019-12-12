+++
showonlyimage = false
draft = false
image = ""
date  = "2019-11-01"
title = "Ego-centric Navigation: the egocircle"
tags  = ["PiPS"]
+++

**Abstract:** Our first attempt at integrating the PiPS concept with
a local-global navigation scheme.  It modified the DWA planner in the
ROS Move Base package.  The procedure required defining the _egocircle_
representation and using it as a body-frame collision and cost-map
reference for planning. Both PiPS and the egocircle lead to linear
scaling in sensor throughput and collision checking, which is confirmed
through computational profiling and compared to other collision
checking methods.
<!--more-->

More details will be forthcoming.[^1]



[^1]: J.S. Smith, S. Feng, F. Lyu, P.A. Vela. "Real-Time Egocentric
Navigation Using 3D Sensing." In <u>Machine Vision and Navigation</u> ,
O. Sergiyenko, W. Flores-Fuentes, P. Mercorelli (eds.), Springer, 2019.  [book](https://www.springer.com/gp/book/9783030225865)

