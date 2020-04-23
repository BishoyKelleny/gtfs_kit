Changes
=======

4.0.1, 2020-04-24
-----------------
- Bugfix: got ``read_feed()`` working on Windows thanks to `pull request 4 <https://github.com/mrcagney/gtfs_kit/pull/4>`_.


4.0.0, 2020-03-06
-----------------
- Breaking changes: renamed ``list_gtfs()`` to ``list_feed()``, ``read_gtfs()`` to ``read_feed()``, and ``write_gtfs()`` to ``write()`` and made it a Feed method.
- Made ``read_feed()`` accept URLs as requested in `pull request 3 <https://github.com/mrcagney/gtfs_kit/pull/3>`_.


3.0.1, 2020-01-16
-----------------
- Optimized function ``geometrize_routes()`` by ignoring duplicate shapes.


3.0.0, 2020-01-10
-----------------
- Breaking change: improved function ``compute_screen_line_counts()`` to handle multiple screen lines at once.
- Added helper function ``make_ids()``.


2.2.1, 2019-11-07
-----------------
- Bugfix: updated function ``map_trips()`` to heed the ``include_arrows`` parameter.


2.2.0, 2019-10-31
-----------------
- Modularized some by added the functions ``build_aggregate_routes_dict()`` and ``build_aggregate_stops_dict()``.


2.1.0, 2019-10-10
-----------------
- Bugfix: updated ``aggregate_stops()`` to handle parent stations.
- Added optional direction arrows to ``map_trips()``.


2.0.0, 2019-10-04
-----------------
- Improved the fallback algorithm in ``append_dist_to_stop_times()``. Changed the function signature, so this is a major change, hence the major version bump.
- Removed optional direction arrows in ``map_trips()``, because the PolyLineTextPath Folium plugin needed for that seems to be broken.


1.1.1, 2019-09-25
-----------------
- Bugfix: imported ``aggregate_stops()`` as a Feed method.


1.1.0, 2019-09-25
-----------------
- Added ``aggregate_stops()`` function.
- Added optional direction arrows in ``map_trips()``.


1.0.2, 2019-09-20
-----------------
- Bugfix: Fixed CRS in ``geometrize_trips()`` and ``geometrize_routes()`` when ``use_utm=True``.


1.0.1, 2019-09-20
-----------------
- Bugfixed: Fixed occasional indexing error in ``geometrize_stops()`` and ``geometrize_shapes()`` when ``use_utm=True``.


1.0.0, 2019-09-18
-----------------
- First release based on prior work.
