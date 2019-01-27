
## MARS SURFACE DENSITY
#### Capstone of course __Data Management and Visualization__


### _July 27, 2016_

### Abstract
I’m interesting in density of surface of Mars which I hope to achieve from
dataset collected in theMars Crater Codebook

## 1. Mars surface study

The formation of meteor(impact) crater consists from 3 phases/stages [3]:

1. Contact and compression
2. Excavation
3. Modification and collapse

On all of above stages deformation of the surface take place,but only of the
1-st stage - due to impact. Exactly on this stage deformationof surface described
by __Newton’s approximation for the impact depth__[4]: <img style="vertical-align: middle" src="https://latex.codecogs.com/gif.latex?&space;D&space;=&space;L\dfrac{A}{B}" />, where
D,L,A,B are crater depth, meteor size, Mars and meteor density respectively.
In this way, depth of craters depend from surface density and, as mentioned in
[4], the lower the density the lower the depth. More over, [4] claim that depth
to diameter ratio is a constant value is about 1/3 for not too large meteors (¡.e
3-4 km). For giant meteors this ratio significantly less.

As noticed in [3], 92% of meteors in the Solar System are rocks, so we may take
value B as constant,    

<!-- ### $$R=\dfrac{D}{L},\hspace{5em}(1)$$ -->      
<div style="text-align:center" ><img  src="https://latex.codecogs.com/gif.latex?&space;R=\dfrac{D}{L},\hspace{5em}(1)"/></div>

where _D_ - crater depth, _L_ - crater diameter
This expression is normalized depth of crater.
On the other hand expression (_1_) may be written as:

<!-- ### $$R\to F_{1,2,3} +E_t,\hspace{3em}(2)$$ -->
<div style="text-align:center" ><img src="https://latex.codecogs.com/gif.latex?&space;R\to&space;F_{1,2,3}&space;&plus;E_t,\hspace{3em}(2)"/></div>

where: <img src="https://latex.codecogs.com/gif.latex?F_{1,2,3}" style="vertical-align: middle"/> - deformations of 3 phases of impact, <img src="https://latex.codecogs.com/gif.latex?${E_t}$" style="vertical-align: middle"/> - wind erosion (because
Mars does not have any significant kind of erosion)

Wind erosion [2] inversely proportional to surface density, i.e crater depth
will decrease more faster for sand then for rocks. In this wayerosion only
increase effect of deformation and may be left out. So _(2)_ will look as: <img src="https://latex.codecogs.com/gif.latex?$R\to&space;F_{1,2,3}$" style="vertical-align: middle"/> for not too big craters.

On the 1-st stage (contact and penetration) diameter≈size of meteor (L)
but after 3-nd stage it decrease up to 85% of the original size[1].

My **hypothesis** and __topic__ are: 
given magnitudes of diameter and depth of Mars craters build classifier for surface density and using nearest craterscoordinate predict surface density for any point on surface.

## 2. Mars Crater Variables

### 2.1 Variable Names

CRATER.ID, LATITUDE.CIRCLE.IMAGE, LONGITUDE.CIRCLE.IMAGE, DIAM.CICLEI.MAGE, DEPTH.RIMFLOOR.TOPOG

Unique Identifier: CRATER.ID

### 2.2 Variables with Descriptions

- CRATER.ID crater ID for internal sue, based upon the region of the
    planet (1/16ths), the pass under which the crate was identified, ad the
    order in which it was identified
- LATITUDE.CIRCLE.IMAGE latitude from the derived center of a non-linear least-squares circle fit to the vertices selected to manually identify
    the crater rim (units are decimal degrees North)
- LONGITUDE.CIRCLE.IMAGE longitude from the derived center of a
    non-linear least-squares circle fit to the vertices selected to manually iden-
    tify the crater rim (units are decimal degrees East)
- DIAM.CIRCLE.IMAGE diameter from a non-linear least squares circle
    fit to the vertices selected to manually identify the crater rim (units are
    km)
- DEPTH.RIMFLOOR.TOPOG average elevation of each of the manually
    determined N points along (or inside) the crater rim(units are km)

## References

[1] Stuart James Robbins. “Planetary Surface Properties, Cratering Physics,
and the Volcanic History of Mars from a New Global Martian Crater
Database”. 2011.

[2] [Wikipedia. Aeolian processes.](url:https://en.wikipedia.org/wiki/
Aeolian_processes)

[3] [Wikipedia. Impact crater](url:https://en.wikipedia.org/wiki/Impact_crater)

[4] [Wikipedia. Impact depth.](url:https://en.wikipedia.org/wiki/Impact_depth).



