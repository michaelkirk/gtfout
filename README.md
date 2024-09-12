# GTF(S)OUT

Tools for manipulating GTFS files.

This was developed for use in Headway, but might be useful in other contexts
too.


## Current functionality

## Bounds Computation

Compute the bounds of the geometries in a GTFS directory.

## Assume bikes are allowed

There is a *sometimes* used trait in GTFS feeds, which declares whether the
transit route supports bikes. Some routers (like OpenTripPlanner) use this
information to determine if multi-modal bike+bus routing is possible.

The problem is that many transit agencies, while allowing bikes, do not declare
this in their GTFS feeds, so this tool simply assumes that bikes are allowed on
all transit. It's a heavy hammer, I know, but it hasn't been wrong for me yet
in the areas where I support transit routing.

