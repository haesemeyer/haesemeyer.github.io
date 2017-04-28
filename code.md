---
layout: page
title: Code
permalink: /code/
---
Most of my research relies on custom written programs both for data acquisition and analysis.
For the most part the programs I use to acquire data, be it freely swimming zebrafish
behavior, head embedded behavior or imaging, are written in
[C#](https://msdn.microsoft.com/en-us/library/67ef8sbd.aspx). The big advantage of C#
is that it allows to write very fast and well structured code without the use of an
intermediate interpreter. On the other hand C# has very good support for user interface
design which makes writing programs with graphical user interfaces fairly straightforward.

For analysis code I heavily rely on [Python](https://www.python.org/) because of its strong
library support for numerical computation and modeling.

This page introduces some libraries or programs which might be of more general interest.

### ZebraTrack
[ZebraTrack](https://haesemeyer.github.io/ZebraTrack/) is a program for online
tracking of larval zebrafish at high framerates. It provides a user interface to run
experiments as well as a flexible design to allow definition of arbitrary open- and
closed- loop experiments.

{% include image.html
    img="assets/scr/UI_CamImage.png"
    title="ZebraTrack"
    width="400"
    caption="ZebraTrack"
    url="https://haesemeyer.github.io/ZebraTrack/" %}

### RegionSelector
{% include github-link.html link="haesemeyer/RegionSelector" name="RegionSelector" %} is
a python and qt5 based program, tested on OsX and Windows, to annotate regions in 3D image stacks.  
The program supports
named polygon regions with an arbitrary number of vertices. Regions can be propagated
between adjacent slices for faster annotation and can be saved to and loaded from simply
structured hdf5 files.

{% include image.html
    img="assets/scr/RegionSelUI.png"
    title="RegionSelector"
    width="550"
    caption="RegionSelector user interface with a partially annotated zebrafish brain" %}

### MhAPI
{% include github-link.html link="haesemeyer/MhAPI" name="MhAPI" %} bundles code that makes
it easier to write user-interface code, do simple image manipulations, track freely swimming
and head embedded zebrafish as well as control stimuli.
