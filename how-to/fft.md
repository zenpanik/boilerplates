
# Fourier Series/Transforms and its applications (not much theory)

 Also known as harmonic analysis it is very important with great variety of applications in many fields of science, math, engineering and finance. The subject of Fourier series is to analyze periodic phenomenon or in other words patterns that repeat regularily over and over again. The periodicity could be in time - there is a phenomenon that repeats over time (if you wait long enough you will see it again), or it could be in space (image processing).

 Usually there is a signal (in one or many dimensions) that is measured over time and there is certain amount of symmetry observed. So the periodicity could be concequence of that symmetry. For example you can imagine how the Earth is circulating around the Sun. There is a eliptiotic trajectory (orbit) that has circular symmetry. So measuring the sun light will be periodic because if you go around the orbit you will be at the same point.

The problem that Fourier Transform actualy solves is how arbitrary real valued functions could be represented by sums of simpler functions. So the result if an infinite sum of trigonometric functions that are used to model periodic functions. 

# Discrete Fourier Transform and Fast Fourier Transform

It is hard to analytically compute the integrals included in the Fourier Transform for complex input functions. Here is why numerical computations of these is very interesing. That is why the method for DFT has gained popularity and is widely adopted in many fields. There is also a fast version proposed by Cooley and Tukey in 1965 of this method caled Fast Fourier Transform (FFT). 

No Mathematical Formulas here. 

But a great video:
https://www.youtube.com/watch?v=spUNpyF58BY

# Important Characteristics of DFT/FFT

## Sampling Frequency

http://sites.music.columbia.edu/cmc/MusicAndComputers/chapter2/02_03.php

## Spectrum

## Power Spectrum

## Parseval's Theorem

The total power in the two domains (time/frequency) are equal.

# Python

## Jupyter Notebook