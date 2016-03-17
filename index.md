---
title       : Cognitive control of eye movements
subtitle    : A model of voluntary and involuntary saccade generation
author      : Ryan M. Hope
job         : Rensselaer Polytechnic Institute
biglogo     : rpi_logo.png
logo        : cogworks_logo.png
framework   : io2012
highlighter : highlight.js
hitheme     : tomorrow
widgets     : [mathjax]
mode        : selfcontained
knit        : slidify::knit2slides

---



## Voluntary vs. involuntary eye movements

+ Humans make on average 1-4 saccades every second
    - thats 10s to 100s of thousands of saccades per day
    - how many are deliberately planned?
    
+ Humans feel like they can VOLUNTARILY move their eyes:
    - to any location
    - at any time
    
+ Certain circumstances absolutely INVOLUNTARILY saccades:
    - e.g. the sudden onset of a visual stimulus

---

## Evidence supporting automatic saccade timing

+ corrective eye movements (aka glissades)
    - short intersaccadic intervals
    - no intersaccadic interval
    - overlapping saccades

+ fixational eye movements (aka microsaccades)
    - reduce image fading from photoreceptor fatigue
    - possibly related to shifts of attention
    - follows main-sequence

+ smooth pursuit
    - lots of small regularly spaced unconscious saccades

---

## Short intersaccadic intervals

![plot of chunk msisi](assets/fig/msisi-1.png)

---

## Overlapping saccades and glissades

![plot of chunk osg](assets/fig/osg-1.png)

---

## Smooth pursuit

![plot of chunk sp](assets/fig/sp-1.png)

--- .segue .dark .quote

<center><ss>How does the sense of voluntary control emerge from an oculomotor control system based on automatic saccade timing?</ss></center>

---

## The (C)ontrolled (R)andom-walk with (I)nhibition for (S)accade (P)lanning model

![plot of chunk crisp1](assets/fig/crisp1-1.png)

---

## CRISP control mechanisms

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2-1.png)

---

## CRISP DEVS (Discrete Event System Specification)

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3-1.png)

https://github.com/RyanHope/PyeMovements/blob/master/crisp.py

https://simpy.readthedocs.org/en/latest

--- .segue .dark .quote

## The Experiment

--- &twocol

## Mixed-block antisaccade task

*** =left 

+ 23 subjects
+ 480 trials split by 12 blocks
    - 20 anti / 20 pro per block
    - Dropped all trials with blinks between fixation point offset
    and first saccade

*** =right

![plot of chunk unnamed-chunk-4](assets/fig/unnamed-chunk-4-1.png)

---

## Saccade response accuracy

![plot of chunk sra](assets/fig/sra-1.png)

---

## Saccade latency

![plot of chunk sl](assets/fig/sl-1.png)

---

## Saccade amplitude

![plot of chunk sa](assets/fig/sa-1.png)

---

## Main sequence

![plot of chunk ms](assets/fig/ms-1.png)

--- .segue .dark .quote

## Models \& Simulations

--- .segue .dark .quote

## Simulation 1

---

## Sim1 saccade latency (prosaccade trials)

![plot of chunk s1slp](assets/fig/s1slp-1.png)

---

## Sim1 saccade latency (antisaccade trials)

![plot of chunk s1sla](assets/fig/s1sla-1.png)

---

## Sim1 cluster analysis

![plot of chunk s1ca](assets/fig/s1ca-1.png)

--- .segue .dark .quote

## Simulation 2

---

## Sim2 saccade response accuracy

![plot of chunk s2ra](assets/fig/s2ra-1.png)

---

## Sim2 saccade latency (prosaccade trials)

![plot of chunk s2slp](assets/fig/s2slp-1.png)

---

## Sim2 saccade latency (antisaccade trials)

![plot of chunk s2sla](assets/fig/s2sla-1.png)

---

## Sim2 cluster analysis

![plot of chunk s2ca](assets/fig/s2ca-1.png)
