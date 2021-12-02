# TR-FTDT
> Time Reversal Algorithm with Finite-Difference Time-Domain Method
Software implementation of a microwave imaging technique for breast cancer early diagnosis. 

This repo contains Matlab files I have wrote for my graduation project. This project is based on a paper by [P. Kosmas & C.M. Rappaport](https://ieeexplore.ieee.org/document/1463350).

## How it Works?

- Run `WithTumor.m` and `WithoutTumor.m`. These will collect data from 3D simulated tissue. Collected data is exported to `withtumor.mat` and `withouttumor.mat` files.
- Then run `TR.m` file. This is time reversal algorithm. It will take difference signals from previous two simulations. Filters the signal using some special filter, then propagates it in the same environment backwards in time. 2D slice of electrical Field in the 3D environment is visualised in every n iterations. Hopefully you can see tumor in the visual.

## Content

### diel_tumor_lin.m

Tumor inside dielectric medium observed by linear antenna array

### diel_no_tumor_lin.m

Dielectric medium without tumor observed by linear array

### TR_lin.m

Time Reversal of linear array, dielectric medium

### TR.m

Time Reversal of linear array, conductive medum

### WithTumor.m

Tumor inside conductive medium observed by linear array

### WithoutTumor.m

Conductive medium without tumor observed by linear array


## Old Content

### bitirme1.m

2D lossless FTDT causal-time simulation

### bitirme2.m

same but with parameters choosen by Kosmas et al.

### bitirme3.m

2D lossy simulation

### bitirme4.m

2D lossy simulation with tissue material

### Maxwell3D.m

3D lossless sim

### Material3D.m

3D sim with material

### Conductivity.m

3D lossy with

### Other scripts

Retrieved from Pelin Cerav's work. 


