# Comparing `tmp/nfl_veripy-0.0.1.tar.gz` & `tmp/nfl_veripy-0.0.1a4.tar.gz`

## Comparing `nfl_veripy-0.0.1.tar` & `nfl_veripy-0.0.1a4.tar`

### file list

```diff
@@ -1,381 +1,381 @@
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/.dockerignore
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/.gitmodules
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/mypy.ini
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/__init__.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/example.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/README.md
--rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator/us.pkl
--rw-r--r--   0        0        0    38879 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl
--rw-r--r--   0        0        0    19521 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl
--rw-r--r--   0        0        0    38881 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl
--rw-r--r--   0        0        0   200000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/duffing/us.csv
--rw-r--r--   0        0        0   406460 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/duffing/xs.csv
--rw-r--r--   0        0        0  3585776 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/iss/iss.mat
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/iss/us.csv
--rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/iss/xs.csv
--rw-r--r--   0        0        0   119223 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/quadrotor/us.pkl
--rw-r--r--   0        0        0   238287 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/acc23_/testing
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/backreach.yaml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/duffing.yaml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/iss.yaml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig5.yaml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/jax/jax_fwd_quadrotor.yaml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp.yaml
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/ojcsys23/di_breach.yaml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/ojcsys23/di_hybreach.yaml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/README.md
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    59120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json
--rw-r--r--   0        0        0    87584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json
--rw-r--r--   0        0        0   155728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
--rw-r--r--   0        0        0   290336 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json
--rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json
--rw-r--r--   0        0        0    32240 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json
--rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json
--rw-r--r--   0        0        0    28736 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json
--rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json
--rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json
--rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json
--rw-r--r--   0        0        0    44368 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json
--rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/default/model.h5
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/default/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json
--rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/default/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/default/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json
--rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json
--rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json
--rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Pendulum/default/model.h5
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Pendulum/default/model.json
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/default/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/default/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json
--rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/test/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/test/model.json
--rw-r--r--   0        0        0    43079 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt
--rw-r--r--   0        0        0   300928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json
--rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json
--rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json
--rw-r--r--   0        0        0   843480 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/default/model.h5
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/default/note.txt
--rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb
--rw-r--r--   0        0        0     8788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.data-00000-of-00001
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.index
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unity/default/model.h5
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unity/default/model.json
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy/model.json
--rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy2/model.json
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy3/model.json
--rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy4/model.json
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/analyzers/Analyzer.py
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/analyzers/ClosedLoopAnalyzer.py
--rw-r--r--   0        0        0    19097 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/analyzers/__init__.py
--rw-r--r--   0        0        0    36595 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/constraints/ClosedLoopConstraints.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/constraints/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DiscreteQuadrotor.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DoubleIntegrator.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DoubleIntegratorx4.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Duffing.py
--rw-r--r--   0        0        0    21852 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Dynamics.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/GroundRobotDI.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/GroundRobotSI.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/ISS.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/ISS_discrete.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Pendulum.py
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Quadrotor.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Quadrotor_8D.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Quadrotor_v0.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Taxinet.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Unicycle.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Unity.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/dynamics/__init__.py
--rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/elements/Element.py
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/elements/GuidedElement.py
--rw-r--r--   0        0        0    12723 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/elements/OptGuidedElement.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/elements/__init__.py
--rw-r--r--   0        0        0    33527 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/experiments/ClosedLoopExperiments.py
--rw-r--r--   0        0        0    36029 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/experiments/backward_experiments.py
--rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/experiments/experiments.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/experiments/expts.py
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py
--rw-r--r--   0        0        0    19044 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopNickPartitioner.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopNoPartitioner.py
--rw-r--r--   0        0        0    28347 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py
--rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/NoPartitioner.py
--rw-r--r--   0        0        0    31837 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/Partitioner.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/SimGuidedPartitioner.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/UnGuidedPartitioner.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/UniformPartitioner.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/partitioners/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/AutoLIRPA.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopAUTOLIRPAPropagator.py
--rw-r--r--   0        0        0    38393 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopCROWNIBPCodebasePropagator.py
--rw-r--r--   0        0        0    36482 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopPropagator.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py
--rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/CrownIBP.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/Propagator.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/SDP.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/propagators/__init__.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/alpha-beta-crown_test.py
--rw-r--r--   0        0        0    25699 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/closed_loop_verification_jax.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/controller_generation.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/create_training_dataset.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/debug_polytope.py
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/debug_prop.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/duffing_data_generating.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/generate_rpm_data.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/iss_data_generating.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/mpc.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/nn.py
--rw-r--r--   0        0        0    23321 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/nn_bounds.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/nn_closed_loop.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/nn_jax.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/optimization_utils.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/plot_rect_prism.py
--rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/reach_sdp.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/run_overt.jl
--rw-r--r--   0        0        0    11928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/src/nfl_veripy/utils/utils.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/tests/test.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/LICENSE
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/README.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.dockerignore
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.gitmodules
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/mypy.ini
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/__init__.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/example.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/README.md
+-rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/us.pkl
+-rw-r--r--   0        0        0    38879 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl
+-rw-r--r--   0        0        0    19521 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl
+-rw-r--r--   0        0        0    38881 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl
+-rw-r--r--   0        0        0   200000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/us.csv
+-rw-r--r--   0        0        0   406460 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/xs.csv
+-rw-r--r--   0        0        0  3585776 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/iss.mat
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/us.csv
+-rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/xs.csv
+-rw-r--r--   0        0        0   119223 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/us.pkl
+-rw-r--r--   0        0        0   238287 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/acc23_/testing
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/backreach.yaml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/duffing.yaml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/iss.yaml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig5.yaml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_quadrotor.yaml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp.yaml
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/ojcsys23/di_breach.yaml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/ojcsys23/di_hybreach.yaml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/README.md
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    59120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json
+-rw-r--r--   0        0        0    87584 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json
+-rw-r--r--   0        0        0   155728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
+-rw-r--r--   0        0        0   290336 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json
+-rw-r--r--   0        0        0    23088 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json
+-rw-r--r--   0        0        0    32240 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json
+-rw-r--r--   0        0        0    23280 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json
+-rw-r--r--   0        0        0    28736 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json
+-rw-r--r--   0        0        0    33136 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json
+-rw-r--r--   0        0        0    33328 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json
+-rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json
+-rw-r--r--   0        0        0    44368 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json
+-rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.h5
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    26688 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json
+-rw-r--r--   0        0        0    24040 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json
+-rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.h5
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.json
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json
+-rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.json
+-rw-r--r--   0        0        0    43079 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt
+-rw-r--r--   0        0        0   300928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json
+-rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json
+-rw-r--r--   0        0        0    21520 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    27048 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    32896 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    35856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    38616 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json
+-rw-r--r--   0        0        0   843480 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/default/model.h5
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/default/note.txt
+-rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx
+-rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb
+-rw-r--r--   0        0        0     8788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.data-00000-of-00001
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/variables/variables.index
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json
+-rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.h5
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.json
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.json
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.json
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.json
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.json
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/Analyzer.py
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/ClosedLoopAnalyzer.py
+-rw-r--r--   0        0        0    19097 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/__init__.py
+-rw-r--r--   0        0        0    36595 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/constraints/ClosedLoopConstraints.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/constraints/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DiscreteQuadrotor.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegrator.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorx4.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Duffing.py
+-rw-r--r--   0        0        0    21852 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Dynamics.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotDI.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotSI.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS_discrete.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Pendulum.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_8D.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_v0.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Taxinet.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unicycle.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unity.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/__init__.py
+-rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/Element.py
+-rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/GuidedElement.py
+-rw-r--r--   0        0        0    12723 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/OptGuidedElement.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/elements/__init__.py
+-rw-r--r--   0        0        0    33527 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/ClosedLoopExperiments.py
+-rw-r--r--   0        0        0    36029 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/backward_experiments.py
+-rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/experiments.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/expts.py
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py
+-rw-r--r--   0        0        0    19044 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopNickPartitioner.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopNoPartitioner.py
+-rw-r--r--   0        0        0    28347 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py
+-rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/NoPartitioner.py
+-rw-r--r--   0        0        0    31837 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/Partitioner.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/SimGuidedPartitioner.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UnGuidedPartitioner.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UniformPartitioner.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/AutoLIRPA.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopAUTOLIRPAPropagator.py
+-rw-r--r--   0        0        0    38393 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopCROWNIBPCodebasePropagator.py
+-rw-r--r--   0        0        0    36482 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopPropagator.py
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py
+-rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/CrownIBP.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/Propagator.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/SDP.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/__init__.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/alpha-beta-crown_test.py
+-rw-r--r--   0        0        0    25699 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/closed_loop_verification_jax.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/controller_generation.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/create_training_dataset.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_polytope.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_prop.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/duffing_data_generating.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/generate_rpm_data.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/iss_data_generating.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/mpc.py
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn.py
+-rw-r--r--   0        0        0    23321 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_bounds.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_closed_loop.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_jax.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/optimization_utils.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/plot_rect_prism.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/reach_sdp.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/run_overt.jl
+-rw-r--r--   0        0        0    11928 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/src/nfl_veripy/utils/utils.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/tests/test.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/README.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     9057 2020-02-02 00:00:00.000000 nfl_veripy-0.0.1a4/PKG-INFO
```

### Comparing `nfl_veripy-0.0.1/.gitlab-ci.yml` & `nfl_veripy-0.0.1a4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/.gitmodules` & `nfl_veripy-0.0.1a4/.gitmodules`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/mypy.ini` & `nfl_veripy-0.0.1a4/mypy.ini`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/example.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/example.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator/us.pkl` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/us.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator/xs.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/us.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/double_integrator2/xs.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/duffing/us.csv` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/us.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/duffing/xs.csv` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/duffing/xs.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/iss/iss.mat` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/iss.mat`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/iss/us.csv` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/us.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/iss/xs.csv` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/iss/xs.csv`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/quadrotor/us.pkl` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/us.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/datasets/quadrotor/xs.pkl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/acc23_/testing` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/acc23_/testing`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/backreach.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/backreach.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/duffing.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/duffing.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/greedy_sim_guided.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/iss.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/iss.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/access21/sim_guided.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig3a.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4a.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4b.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig4c.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/cdc22/fig5.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/cdc22/fig5.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_lp_partition.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig3_reach_sdp_partition.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig4b.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5a.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/icra21/fig5b.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_double_integrator_jit.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/jax/jax_fwd_quadrotor.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/jax/jax_fwd_quadrotor.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_breachlp_iterate.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly1.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/lcss23/fig2_driphpoly5.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/ojcsys23/di_breach.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/ojcsys23/di_breach.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/example_configs/ojcsys23/di_hybreach.yaml` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/example_configs/ojcsys23/di_hybreach.yaml`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_100_100/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_128_128_128/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_256_256/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_0/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_1/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_40/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_6/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_7/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_8/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_40_40_9/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_50_50/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_0/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_1/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_6/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_7/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_8/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_60_60_9/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_64_64/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_80_80/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/discrete_quad_avoid_origin_maneuver_fast_test2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/quad_avoid_origin_maneuver_fast/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DiscreteQuadrotor/test3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/history.p`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/diverse_16_16/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegrator/double_integrator_test_5_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/DoubleIntegratorx4/simple_4_DI/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/default/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Duffing/duffing_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotDI/ground_robot_DI_avoid_origin_maneuver_velocity_update/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_complex_potential_field5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/buggy_simple_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/complex_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/GroundRobotSI/go_straight_complex_potential_field/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/default/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/1/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/2/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_10_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/ISS/iss_backup/3_continuous/iss_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Pendulum/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Pendulum/default/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Pendulum/default/single_pendulum_small_controller.torch`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/default/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/discrete_quad_avoid_origin_maneuver_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_small/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/test/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor/test/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor/test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/intermediate_policy_0.pt`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_8D/sim_data.npy`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/avoid_origin_maneuver/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/discrete_quad_avoid_origin_maneuver_2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_small/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/quadrotor_test_5_5_5_5_5_5_5_5_5_5/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Quadrotor_v0/test/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/TinyTaxiNet.onnx`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/from_pb/saved_model.pb`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Taxinet/to_pb/saved_model.pb`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/drive_in_circle_controller/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unicycle/sine_wave_controller/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unity/default/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/Unity/default/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/Unity/default/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy2/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy2/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy3/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy3/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.h5`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/_static/models/debug/corner_policy4/model.json` & `nfl_veripy-0.0.1a4/src/nfl_veripy/_static/models/debug/corner_policy4/model.json`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/analyzers/Analyzer.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/Analyzer.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/analyzers/ClosedLoopAnalyzer.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/ClosedLoopAnalyzer.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/analyzers/ClosedLoopBackwardAnalyzer.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/constraints/ClosedLoopConstraints.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/constraints/ClosedLoopConstraints.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/constraints/__init__.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DiscreteQuadrotor.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DiscreteQuadrotor.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DoubleIntegrator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegrator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorOutputFeedback.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/DoubleIntegratorx4.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/DoubleIntegratorx4.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Duffing.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Duffing.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Dynamics.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Dynamics.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/GroundRobotDI.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotDI.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/GroundRobotSI.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/GroundRobotSI.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/ISS.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/ISS_discrete.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/ISS_discrete.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Pendulum.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Pendulum.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Quadrotor.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/QuadrotorOutputFeedback_v0.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Quadrotor_8D.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_8D.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Quadrotor_v0.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Quadrotor_v0.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Taxinet.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Taxinet.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Unicycle.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unicycle.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/Unity.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/Unity.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/dynamics/__init__.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/elements/Element.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/elements/Element.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/elements/GuidedElement.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/elements/GuidedElement.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/elements/OptGuidedElement.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/elements/OptGuidedElement.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/experiments/ClosedLoopExperiments.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/ClosedLoopExperiments.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/experiments/backward_experiments.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/backward_experiments.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/experiments/experiments.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/experiments.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/experiments/expts.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/experiments/expts.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/AdaptiveGreedySimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/BoundarySimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopGreedySimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopNickPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopNickPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopNoPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopNoPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopSimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUnGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/ClosedLoopUniformPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/GreedySimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/NoPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/NoPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/Partitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/Partitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/SimGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/SimGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/UnGuidedPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UnGuidedPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/UniformPartitioner.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/UniformPartitioner.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/partitioners/__init__.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/partitioners/__init__.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/AutoLIRPA.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/AutoLIRPA.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopAUTOLIRPAPropagator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopAUTOLIRPAPropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopCROWNIBPCodebasePropagator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopCROWNIBPCodebasePropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopJaxVerifyPropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopOVERTPropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopPropagator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopPropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSDPPropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/ClosedLoopSeparablePropagator.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/CrownIBP.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/CrownIBP.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/SDP.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/SDP.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/propagators/__init__.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/propagators/__init__.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/alpha-beta-crown_test.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/alpha-beta-crown_test.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/closed_loop_verification_jax.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/closed_loop_verification_jax.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/controller_generation.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/controller_generation.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/create_training_dataset.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/create_training_dataset.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/debug_polytope.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_polytope.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/debug_prop.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/debug_prop.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/duffing_data_generating.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/duffing_data_generating.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/generate_rpm_data.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/generate_rpm_data.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/iss_data_generating.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/iss_data_generating.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/mpc.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/mpc.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/nn.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/nn_bounds.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_bounds.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/nn_closed_loop.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_closed_loop.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/nn_jax.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/nn_jax.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/optimization_utils.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/plot_rect_prism.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/plot_rect_prism.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/reach_sdp.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/reach_sdp.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/run_overt.jl` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/run_overt.jl`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/src/nfl_veripy/utils/utils.py` & `nfl_veripy-0.0.1a4/src/nfl_veripy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/tests/test.py` & `nfl_veripy-0.0.1a4/tests/test.py`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/.gitignore` & `nfl_veripy-0.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/LICENSE` & `nfl_veripy-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `nfl_veripy-0.0.1/README.md` & `nfl_veripy-0.0.1a4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-# nfl_veripy: Formal Verification of Neural Feedback Loops (NFLs)
-
 ## Updates
 
-- **2023-04-21:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
+- **2023-04-19:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
 - **2023-04-13:** Add new jax-based propagators, including some from [`DRIP` paper](https://arxiv.org/abs/2212.04646). Cleaned up implementation of BReach-LP and HyBReach-LP from OJCSYS paper.
 - **2022-06-20:** Add new backprojection code from [`BReach-LP` paper](https://arxiv.org/abs/2204.08319). More info [here](/docs/_static/cdc22/cdc22.md)
 - **2022-05-09:** Add new N-Step `ClosedLoopPropagator`. Rather than recursively computing reachable sets (suffers from the wrapping effect), we see improved performance by solving an LP directly for the reachable set N steps in the future. You can experiment with this using the `CROWNNStep` flag in `nfl_veripy/example.py`.
 - **2022-05-09:** Add new MILP-based `ClosedLoopPropagator`, using [`OVERT`](https://github.com/sisl/OVERTVerify.jl). Note that this component requires a Julia installation, and we pass data between Python and Julia using a lightweight local HTTP server. More info [here](/docs/_static/other.md).
 
 ## About
 
-`nfl_veripy` is a Python codebase for formal safety verification of neural feedback loops (NFLs).
-An example of an NFL is a dynamical system controlled by a neural network policy.
+### `nfl_veripy`: Closed-Loop Analysis (NNs in feedback loops) -- includes Reach-LP and BReach-LP
 
-Currently, **`nfl_veripy` handles problems such as:**
+**Handles problems such as:**
 - Given a set of possible initial states, a trained NN controller, and a known dynamics model, compute outer bounds on the set of possible future states (**forward reachable sets**).
 - Given a set of terminal states, a trained NN controller, and a known dynamics model, compute inner/outer bounds on the set of possible initial states that will/won't lead to the terminal state set (**backprojection sets**).
 
 For more info, please see [this README](/docs/_static/access21/access21.md) and [this README](/docs/_static/cdc22/cdc22.md).
 
 ## Setup
 
 If you just want to run the code, you can simply install our package via pip:
 ```bash
-pip install \
-    "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" \
+pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" \
     "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git" \
     nfl_veripy
 ```
 
+Aside: We acknowledge that the above method for installing `jax_verify` and `crown_ibp` (dependencies of `nfl_veripy`) in the above way is a little unconventional.
+It would be better to simply include these as dependencies of `nfl_veripy` and let pip find those packages, but (a) those packages are not available (or are too outdated) on PyPI, and (b) it is not allowed to include dependencies with direct URLs when releasing a package on PyPI.
+If there's a better way of doing this we would love to hear about it!
+
 ### Simple Examples
 
 Compute forward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/icra21/fig3_reach_lp.yaml
 ```
 
 Compute backward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/ojcsys23/di_breach.yaml
 ```
 
+### Jupyter Notebooks
+
+Please see the `jupyter_notebooks` folder for an interactive version of the above examples.
+
 ### Replicate plots from the papers:
 
 * LCSS/ACC '21: [README](/docs/_static/lcss21/lcss21.md)
 * ICRA '21: [README](/docs/_static/icra21/icra21.md)
 * IEEE Access '21: [README](/docs/_static/access21/access21.md)
 * CDC '22: [README](/docs/_static/cdc22/cdc22.md)
 * ACC '23 (to appear): Coming soon!
@@ -70,14 +74,21 @@
 We build on excellent open-source repositories from the neural network analysis community. These repositories are imported as Git submodules or re-implemented in Python here, with some changes to reflect the slightly different problem statements:
 * [`auto_LIRPA`](https://github.com/KaidiXu/auto_LiRPA)
 * [`crown_ibp`](https://github.com/huanzhang12/CROWN-IBP)
 * [`robust_nn`](https://github.com/arobey1/RobustNN)
 * [`nnv`](https://github.com/verivital/nnv)
 * [`jax_verify`](https://github.com/deepmind/jax_verify)
 
+
+## TODOS:
+
+- [ ] add rtdocs (auto-fill code snippets from test files)
+- [ ] add installation instructions & tests for julia code
+
+
 ## Developer Setup
 
 If you want to work directly with the source code, here is how we set up our development environments.
 
 ### Get the code
 
 ```bash
@@ -98,8 +109,20 @@
 ```
 
 Install the various python packages in this repo in editable mode (`-e`):
 ```bash
 python -m pip install -e third_party/crown_ibp third_party/jax_verify third_party/auto_LiRPA .
 ```
 
-You're good to go!
+You're good to go!
+
+## packaging info
+
+```bash
+cd nfl_veripy
+python -m build
+python -m twine upload --repository testpypi dist/nfl_veripy-0.0.1a0*
+
+python -m pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git"
+python -m pip install --extra-index-url https://test.pypi.org/simple/ nfl-veripy==0.0.1.a3
+
+```
```

### Comparing `nfl_veripy-0.0.1/pyproject.toml` & `nfl_veripy-0.0.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nfl_veripy"
-version = "0.0.1"
+version = "0.0.1a4"
 authors = [
     { name = "Michael Everett", email = "m.everett@northeastern.edu" },
     { name = "Nicholas Rober", email = "nrober@mit.edu" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `nfl_veripy-0.0.1/PKG-INFO` & `nfl_veripy-0.0.1a4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfl_veripy
-Version: 0.0.1
+Version: 0.0.1a4
 Summary: A small example package
 Project-URL: repository, https://github.com/mit-acl/nn_robustness_analysis.git
 Author-email: Michael Everett <m.everett@northeastern.edu>, Nicholas Rober <nrober@mit.edu>
 License: MIT License
         
         Copyright (c) 2021 MIT Aerospace Controls Lab
         
@@ -46,57 +46,61 @@
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tabulate
 Requires-Dist: torch
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-# nfl_veripy: Formal Verification of Neural Feedback Loops (NFLs)
-
 ## Updates
 
-- **2023-04-21:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
+- **2023-04-19:** Major cleanup and re-branding of repo, released PyPi package for easier usability!
 - **2023-04-13:** Add new jax-based propagators, including some from [`DRIP` paper](https://arxiv.org/abs/2212.04646). Cleaned up implementation of BReach-LP and HyBReach-LP from OJCSYS paper.
 - **2022-06-20:** Add new backprojection code from [`BReach-LP` paper](https://arxiv.org/abs/2204.08319). More info [here](/docs/_static/cdc22/cdc22.md)
 - **2022-05-09:** Add new N-Step `ClosedLoopPropagator`. Rather than recursively computing reachable sets (suffers from the wrapping effect), we see improved performance by solving an LP directly for the reachable set N steps in the future. You can experiment with this using the `CROWNNStep` flag in `nfl_veripy/example.py`.
 - **2022-05-09:** Add new MILP-based `ClosedLoopPropagator`, using [`OVERT`](https://github.com/sisl/OVERTVerify.jl). Note that this component requires a Julia installation, and we pass data between Python and Julia using a lightweight local HTTP server. More info [here](/docs/_static/other.md).
 
 ## About
 
-`nfl_veripy` is a Python codebase for formal safety verification of neural feedback loops (NFLs).
-An example of an NFL is a dynamical system controlled by a neural network policy.
+### `nfl_veripy`: Closed-Loop Analysis (NNs in feedback loops) -- includes Reach-LP and BReach-LP
 
-Currently, **`nfl_veripy` handles problems such as:**
+**Handles problems such as:**
 - Given a set of possible initial states, a trained NN controller, and a known dynamics model, compute outer bounds on the set of possible future states (**forward reachable sets**).
 - Given a set of terminal states, a trained NN controller, and a known dynamics model, compute inner/outer bounds on the set of possible initial states that will/won't lead to the terminal state set (**backprojection sets**).
 
 For more info, please see [this README](/docs/_static/access21/access21.md) and [this README](/docs/_static/cdc22/cdc22.md).
 
 ## Setup
 
 If you just want to run the code, you can simply install our package via pip:
 ```bash
-pip install \
-    "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" \
+pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" \
     "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git" \
     nfl_veripy
 ```
 
+Aside: We acknowledge that the above method for installing `jax_verify` and `crown_ibp` (dependencies of `nfl_veripy`) in the above way is a little unconventional.
+It would be better to simply include these as dependencies of `nfl_veripy` and let pip find those packages, but (a) those packages are not available (or are too outdated) on PyPI, and (b) it is not allowed to include dependencies with direct URLs when releasing a package on PyPI.
+If there's a better way of doing this we would love to hear about it!
+
 ### Simple Examples
 
 Compute forward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/icra21/fig3_reach_lp.yaml
 ```
 
 Compute backward reachable sets for a closed-loop system with a pre-trained NN control policy:
 ```bash
 python -m nfl_veripy.example --config example_configs/ojcsys23/di_breach.yaml
 ```
 
+### Jupyter Notebooks
+
+Please see the `jupyter_notebooks` folder for an interactive version of the above examples.
+
 ### Replicate plots from the papers:
 
 * LCSS/ACC '21: [README](/docs/_static/lcss21/lcss21.md)
 * ICRA '21: [README](/docs/_static/icra21/icra21.md)
 * IEEE Access '21: [README](/docs/_static/access21/access21.md)
 * CDC '22: [README](/docs/_static/cdc22/cdc22.md)
 * ACC '23 (to appear): Coming soon!
@@ -122,14 +126,21 @@
 We build on excellent open-source repositories from the neural network analysis community. These repositories are imported as Git submodules or re-implemented in Python here, with some changes to reflect the slightly different problem statements:
 * [`auto_LIRPA`](https://github.com/KaidiXu/auto_LiRPA)
 * [`crown_ibp`](https://github.com/huanzhang12/CROWN-IBP)
 * [`robust_nn`](https://github.com/arobey1/RobustNN)
 * [`nnv`](https://github.com/verivital/nnv)
 * [`jax_verify`](https://github.com/deepmind/jax_verify)
 
+
+## TODOS:
+
+- [ ] add rtdocs (auto-fill code snippets from test files)
+- [ ] add installation instructions & tests for julia code
+
+
 ## Developer Setup
 
 If you want to work directly with the source code, here is how we set up our development environments.
 
 ### Get the code
 
 ```bash
@@ -150,8 +161,20 @@
 ```
 
 Install the various python packages in this repo in editable mode (`-e`):
 ```bash
 python -m pip install -e third_party/crown_ibp third_party/jax_verify third_party/auto_LiRPA .
 ```
 
-You're good to go!
+You're good to go!
+
+## packaging info
+
+```bash
+cd nfl_veripy
+python -m build
+python -m twine upload --repository testpypi dist/nfl_veripy-0.0.1a0*
+
+python -m pip install "jax_verify @ git+https://gitlab.com/mit-acl/ford_ugvs/jax_verify.git" "crown_ibp @ git+https://gitlab.com/mit-acl/ford_ugvs/crown_ibp.git"
+python -m pip install --extra-index-url https://test.pypi.org/simple/ nfl-veripy==0.0.1.a3
+
+```
```

