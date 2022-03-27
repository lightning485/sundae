# Sundae toy data generator
This is a basic attempt on a Blender-based generator of sundaes for use as toy data for educational purposes.
Because I am new to the geometry nodes, the solution is not elegant yet.

## Description
A geometry node system is set up for the generation of sundaes. It creates:
* A cup with corners and random rotation
* Balls with random offset

Rendered are:
* Gray-scale image (panoramic camera)
* 16 bit Depth image (panoramic camera, i.e. with equal angle steps per pixel like such as from a laser scanner)

![](https://raw.githubusercontent.com/lightning485/sundae/main/I0001.JPG)
![](https://raw.githubusercontent.com/lightning485/sundae/main/D0001.JPG)

For the panoramic camera, the cycles renderer is used.
The ice balls are icospheres with high subdivisions.
Both these things make it slow. You can change back to the eevee renderer, or decrease the subdivisions (in the node system)

### Node system
![](https://raw.githubusercontent.com/lightning485/sundae/main/screenshot_blender_geometry.JPG)

### Render settings
![](https://raw.githubusercontent.com/lightning485/sundae/main/screenshot_blender_compositing.JPG)