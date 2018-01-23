# NukePublic
Public Nuke Snippits created by Mads Hagbarth Damsbo.


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


