# tilingutils
Magik utilities for creating tiling configurations for the [tilecacher](https://github.com/OpenSmallworld/nv-tilecacher).

The key utility is in tile_boundary_generator.magik, which defines a Magik calls called tile_boundary_generator. This class provides a method generate_tile_config(), which will use the current view of a running application to calculate a bounding area for a tilecacher config file. This utility was used to generate a set of config files for customer wire centers, both in "simple" and "complex" forms (see comments in the code).

The other Magik file in this repo (generate_cache_list.magik) is a script that was used at a customer to generate a set of tilecacher commands for pre-population of "priority" wire centers supplied by the customer.