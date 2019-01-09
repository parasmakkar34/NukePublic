# NukePublic
Public Nuke Snippits created by Mads Hagbarth Damsbo.


https://github.com/Malu05/NukePublic/blob/master/timelineHotkeys.py


## [timelineHotkeys.py](/timelineHotkeys.py)
This is a basic version of the [View Manager](https://vimeo.com/299745801) that i created back in 2018. It adds a button to the viewer that let you set "hotkeys" for certain frame numbers, frame ranges, nodes, settings and such.

## [RGB2HSP.nk](/RGB2HSP.nk)
This is a node that can convert RGB into HSP and vice versa.
HSP is a colorspace created by [Darel Rex Finley](http://alienryderflex.com/hsp.html), that work much like HSV and HSL with the exception that the luminance is visually percived brightness.


## [BrushReduction.py](/BrushReduction.py)


This script is used to reduce the currently selected roto brush strokes to a minimum.
Using the [Ramer–Douglas–Peucker](https://en.wikipedia.org/wiki/Ramer%E2%80%93Douglas%E2%80%93Peucker_algorithm) algorithm, it takes all the unnecessary points of the brush stroke and removes them.
Due to the slow nature of the roto.remove function in nuke this takes quite a bit of time on big stroke paths (just so you know)

Install: 
```python
import BrushReduction
```
Usage:
With the roto node and brush stroke(s) selected hit the desired menu item in the "Roto" menu.

![GitHub Logo](/Images/reducedCurve.jpg)


## [VectorMorph](/VectorMorph)

This nuke script contains a node that can be used to morph between 2 frames of a sequence using Kronos vectors.
The node automatically morphs and resumes the normal sequence.


