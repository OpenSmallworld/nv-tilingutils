# tilingutils
Magik utilities for creating tiling configurations for the [tilecacher](https://github.build.ge.com/105002616/tilecacher).

The key utility is in tile_boundary_generator.magik, which defines a Magik calls called tile_boundary_generator. This class provides a method generate_tile_config(), which will use the current view of a running application to calculate a bounding area for a tilecacher config file. This utility was used to generate a set of config files for CenturyLink wire centers, both in "simple" and "complex" forms (see comments in the code).

The other Magik file in this repo (generate_cache_list.magik) is a script that was used at CenturyLink to generate a set of tilecacher commands for pre-population of "priority" wire centers supplied by CenturyLink. This does not have general applicability - it is strictly for Centurylink.