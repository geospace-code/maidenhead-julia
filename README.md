# Maidenhead &lt;-&gt; Lat/Lon

`maidenhead` provides a simple, yet effective location hashing
algorithm. Maidenhead allows global location precision down to 750m

Maidenhead provides 4 levels of increasing accuracy

  Level |  Precision
--------|------------
  1     |  World
  2     |  Regional
  3     |  Metropolis
  4     |  City

We also have [Maidenhead conversion for Python](https://github.com/scivision/maidenhead)


### lat lon to Maidenhead locator
```julia
toMaiden(lat, lon, level) 
```
returns a char (len = lvl*2)

### Maidenhead locator to lat lon
```julia
toLoc("AB01cd") 
```
take any string and returns topleft lat, lon of Maidenhead grid square.

