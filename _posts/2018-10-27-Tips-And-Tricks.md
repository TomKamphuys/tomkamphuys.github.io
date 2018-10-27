---
layout: post
title:  "Tips And Tricks"
date:   2018-10-27 11:59:06 +0200
categories: Amp
---

# Tips 'n' Tricks
This blog describes some tips and tricks for working with DIYLC, LTSPICE, Octave/Matlab and some editor. I might make these available to the public on request.

## DIYLC
### Switch the displaying of value and name
Do a search and replace for 
```xml
<display>VALUE</display>
```
and replace by 
```xml
<display>BOTH</display>
```
or vice versa.

## Octave/Matlab

### Calculate tube gain (with cathode bypass cap)
Use `C:\Users\User\Dropbox\cathodeBypassCapacitor.m` to calculate the gain.

### Compare multiple transfer functions from LTSPICE
Use `C:\Users\User\Dropbox\JCM800\jcm800\compareFFT.m`; well, let it inspire you.

### Read transfer function output from LTSPICE into Octave/Matlab
Use `C:\Users\User\Dropbox\JCM800\jcm800\parseSpliceFile.m`.

### Determine transfer function of parts of the amplifier
Use LTSPICE to get transfer functions of the amplifier. Select both the input and output signal of the part you want the transfer function of. You can select more than two and split the entire amplifier in all of its parts. Export the transfer function to .txt and use `C:\Users\User\Dropbox\JCM800\jcm800\splitCircuit.m` to show a graph of the transfer functions. It needs the file name and a sequence which translates the Vn009, Vn027 like nodes into the amp parts. E.g. Vn035 is the input signal, Vn009 is an intermediate signal and Vn016 is the output signal, then the sequence has to be [3, 1, 2] as LTSPICE will put it in this order into the file: Vn009 Vn016 Vn035.
![Example image](/assets/BodePlotSplitCircuit.png)