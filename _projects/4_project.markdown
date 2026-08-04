---
layout: page
title: Real-Time Scheduling
description: Real-time scheduling project.
img: /assets/img/realtimescheduling.jpg
---

While studing in University of Illinois at Urbana-Champaign, my
research aim on supporting the state-dependent real-time scheduling
theory for mission critical systems. One typical example is the
phase array radar installed on fight jets. The scheduling algorithm on
such systems need to take into account the timely requirements and
dynamic workload at the same time.

My doctroal <a
href="https://www.ideals.illinois.edu/handle/2142/81629"
target="blank">thesis</a> considers the general case when a job may
have more than one feasible interval. Such a job is constrained to
execute from start to completion in one of its feasible intervals. The
problem of meeting the timing constraint of such jobs is divided into
three problems: feasible interval determination, feasible interval
selection, and job scheduling. When the deadline of every job is given
as a known time function, there is an optimal feasible interval
determination algorithm: The algorithm determines the start times and
end times of feasible intervals of every job so that the job will
never miss its deadline if the job executes from start to completion
in one of its feasible intervals. When the future values of job
deadlines are unknown, it is not possible to make optimal
determination of feasible intervals. We developed several algorithms
to determine probabilistically feasible interval start times and end
times for each job so that the probability of a job meeting its timing
constraint is no less than a given threshold if it executes from start
to completion in one of its feasible intervals. Given the start times
and end times of feasible intervals, the problem of selecting a
feasible interval for each job in a set of multiple feasible interval
jobs so that all jobs complete in time is NP-hard. The optimal
branch-and-bound algorithm described here can be used when there is
time to compute the schedule.

This research has been extended my other research projects in
following years, including multi-core scheduling, heterogeneous core
scheduling, and fog-cloud scheduling. 
