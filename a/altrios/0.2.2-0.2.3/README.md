# Comparing `tmp/altrios-0.2.2.tar.gz` & `tmp/altrios-0.2.3.tar.gz`

## Comparing `altrios-0.2.2.tar` & `altrios-0.2.3.tar`

### file list

```diff
@@ -1,204 +1,204 @@
--rw-r--r--   0     1001      127     1201 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/Cargo.toml
--rw-r--r--   0     1001      127      784 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/README.md
--rw-r--r--   0     1001      127     2475 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/combo_error.rs
--rw-r--r--   0     1001      127    22917 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/consist_model.rs
--rw-r--r--   0     1001      127     3981 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/consist_sim.rs
--rw-r--r--   0     1001      127    12088 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/consist_utils.rs
--rw-r--r--   0     1001      127     3176 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs
--rw-r--r--   0     1001      127     3606 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/conventional_loco.rs
--rw-r--r--   0     1001      127    12008 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs
--rw-r--r--   0     1001      127    13342 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/loco_sim.rs
--rw-r--r--   0     1001      127    39926 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/locomotive_model.rs
--rw-r--r--   0     1001      127      991 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/mod.rs
--rw-r--r--   0     1001      127      430 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.default.yaml
--rw-r--r--   0     1001      127    14931 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs
--rw-r--r--   0     1001      127     1034 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml
--rw-r--r--   0     1001      127    13407 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs
--rw-r--r--   0     1001      127      348 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/generator.default.yaml
--rw-r--r--   0     1001      127    14475 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs
--rw-r--r--   0     1001      127      213 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/mod.rs
--rw-r--r--   0     1001      127      938 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs
--rw-r--r--   0     1001      127     9907 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml
--rw-r--r--   0     1001      127    30918 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs
--rw-r--r--   0     1001      127      200 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/test.rs
--rw-r--r--   0     1001      127     2790 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/tests.rs
--rw-r--r--   0     1001      127      752 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/mod.rs
--rw-r--r--   0     1001      127     1039 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/tests.rs
--rw-r--r--   0     1001      127     1254 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/imports.rs
--rw-r--r--   0     1001      127     1141 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/lib.rs
--rw-r--r--   0     1001      127     1602 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/lin_search_hint.rs
--rw-r--r--   0     1001      127     8028 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/macros.rs
--rw-r--r--   0     1001      127      482 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/disp_imports.rs
--rw-r--r--   0     1001      127     5431 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/disp_structs.rs
--rw-r--r--   0     1001      127    11495 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/dispatch.rs
--rw-r--r--   0     1001      127     2661 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs
--rw-r--r--   0     1001      127    29031 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/mod.rs
--rw-r--r--   0     1001      127     9721 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/update_times.rs
--rw-r--r--   0     1001      127      281 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/mod.rs
--rw-r--r--   0     1001      127    25666 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs
--rw-r--r--   0     1001      127    36649 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/free_path.rs
--rw-r--r--   0     1001      127     9540 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/mod.rs
--rw-r--r--   0     1001      127     1969 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/prelude.rs
--rw-r--r--   0     1001      127      255 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/pyo3.rs
--rw-r--r--   0     1001      127     1039 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/si.rs
--rw-r--r--   0     1001      127     2613 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/testing.rs
--rw-r--r--   0     1001      127     2129 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/cat_power.rs
--rw-r--r--   0     1001      127     4039 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/elev.rs
--rw-r--r--   0     1001      127     4947 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/heading.rs
--rw-r--r--   0     1001      127     4752 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/link_idx.rs
--rw-r--r--   0     1001      127    23686 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/link_impl.rs
--rw-r--r--   0     1001      127     1387 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/link_old.rs
--rw-r--r--   0     1001      127     1900 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/location.rs
--rw-r--r--   0     1001      127      246 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/locations.csv
--rw-r--r--   0     1001      127      301 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/mod.rs
--rw-r--r--   0     1001      127     4792 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_limit.rs
--rw-r--r--   0     1001      127     3242 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_param.rs
--rw-r--r--   0     1001      127     5971 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_set.rs
--rw-r--r--   0     1001      127      120 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed.rs
--rw-r--r--   0     1001      127      120 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/mod.rs
--rw-r--r--   0     1001      127     6079 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/link_point.rs
--rw-r--r--   0     1001      127      182 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/mod.rs
--rw-r--r--   0     1001      127     2826 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/path_res_coeff.rs
--rw-r--r--   0     1001      127    19995 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/path_tpc.rs
--rw-r--r--   0     1001      127     7804 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/speed_point.rs
--rw-r--r--   0     1001      127     3842 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/train_params.rs
--rw-r--r--   0     1001      127     6200 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/braking_point.rs
--rw-r--r--   0     1001      127     3503 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/friction_brakes.rs
--rw-r--r--   0     1001      127      344 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/mod.rs
--rw-r--r--   0     1001      127     3605 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/rail_vehicle.rs
--rw-r--r--   0     1001      127     1124 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs
--rw-r--r--   0     1001      127      324 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/bearing.rs
--rw-r--r--   0     1001      127      438 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/davis_b.rs
--rw-r--r--   0     1001      127       90 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/mod.rs
--rw-r--r--   0     1001      127     4274 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/path_res.rs
--rw-r--r--   0     1001      127      397 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/rolling.rs
--rw-r--r--   0     1001      127      133 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/method/mod.rs
--rw-r--r--   0     1001      127     2253 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/method/point.rs
--rw-r--r--   0     1001      127     2758 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/method/strap.rs
--rw-r--r--   0     1001      127     1780 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/mod.rs
--rw-r--r--   0     1001      127    13755 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/set_speed_train_sim.rs
--rw-r--r--   0     1001      127    24549 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/speed_limit_train_sim.rs
--rw-r--r--   0     1001      127      443 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/test_rail_vehicles.csv
--rw-r--r--   0     1001      127      182 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/timed_path.rs
--rw-r--r--   0     1001      127    40485 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/train_config.rs
--rw-r--r--   0     1001      127      338 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/train_imports.rs
--rw-r--r--   0     1001      127     8339 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/train_state.rs
--rw-r--r--   0     1001      127    10250 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/traits.rs
--rw-r--r--   0     1001      127     2849 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/uc.rs
--rw-r--r--   0     1001      127    13949 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/utils/mod.rs
--rw-r--r--   0     1001      127     2455 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/utils/val_range.rs
--rw-r--r--   0     1001      127     7292 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/validate.rs
--rw-r--r--   0     1001      127      578 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/Cargo.toml
--rw-r--r--   0     1001      127      707 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/README.md
--rw-r--r--   0     1001      127    10749 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs
--rw-r--r--   0     1001      127    12388 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs
--rw-r--r--   0     1001      127     4077 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs
--rw-r--r--   0     1001      127     2741 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs
--rw-r--r--   0     1001      127      367 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/imports.rs
--rw-r--r--   0     1001      127     1192 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/lib.rs
--rw-r--r--   0     1001      127      571 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs
--rw-r--r--   0     1001      127     3154 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/utilities.rs
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 altrios-0.2.2/rust/altrios-py/Cargo.toml
--rw-r--r--   0     1001      127      586 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-py/README.md
--rw-r--r--   0     1001      127     3080 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-py/src/lib.rs
--rw-r--r--   0     1001      127    63018 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/Cargo.lock
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 altrios-0.2.2/rust/Cargo.toml
--rw-r--r--   0     1001      127     2197 2024-05-14 17:29:53.000000 altrios-0.2.2/pyproject.toml
--rw-r--r--   0     1001      127      766 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/stringline_old.py
--rw-r--r--   0     1001      127      386 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/plot.py
--rw-r--r--   0     1001      127     5988 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/speed_limit_train_sim_demo.py
--rw-r--r--   0     1001      127     4220 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/speed_limit_simple_corr_demo.py
--rw-r--r--   0     1001      127     5592 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/sim_manager_demo.py
--rw-r--r--   0     1001      127     1006 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/version_migration_demo.py
--rw-r--r--   0     1001      127     3410 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/set_speed_simple_corr_demo.py
--rw-r--r--   0     1001      127     3488 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/rollout_demo.py
--rw-r--r--   0     1001      127      111 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/__init__.py
--rw-r--r--   0     1001      127     3903 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/set_speed_train_sim_demo.py
--rw-r--r--   0     1001      127      578 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/test_demos.py
--rw-r--r--   0     1001      127     2357 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/conv_demo.py
--rw-r--r--   0     1001      127     2377 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/bel_demo.py
--rw-r--r--   0     1001      127      278 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/demo_logging.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/py.typed
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/fuel_grid.py
--rw-r--r--   0     1001      127    53858 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/train_planner.py
--rw-r--r--   0     1001      127    52841 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/output_12072022.csv
--rw-r--r--   0     1001      127     8741 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/utilities.py
--rw-r--r--   0     1001      127    16755 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/stringline.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/objectives.py
--rw-r--r--   0     1001      127     1078 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/__init__.py
--rw-r--r--   0     1001      127    41804 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/metric_calculator.py
--rw-r--r--   0     1001      127  1237826 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv
--rw-r--r--   0     1001      127      994 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv
--rw-r--r--   0     1001      127     2025 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv
--rw-r--r--   0     1001      127     1616 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv
--rw-r--r--   0     1001      127    10562 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv
--rw-r--r--   0     1001      127   128287 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrain_model_input_example.csv
--rw-r--r--   0     1001      127      695 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/Default Demand StoBar.csv
--rw-r--r--   0     1001      127       50 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/tpc_input_example.csv
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/__init__.py
--rw-r--r--   0     1001      127      492 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Unit_Empty.yaml
--rw-r--r--   0     1001      127      501 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Unit.yaml
--rw-r--r--   0     1001      127      496 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Manifest_Empty.yaml
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/__init__.py
--rw-r--r--   0     1001      127      511 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Manifest.yaml
--rw-r--r--   0     1001      127      641 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/rail_vehicles.csv
--rw-r--r--   0     1001      127      492 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Intermodal.yaml
--rw-r--r--   0     1001      127      498 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Intermodal_Empty.yaml
--rw-r--r--   0     1001      127      568 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/trains/train_res_temp.yaml
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/trains/__init__.py
--rw-r--r--   0     1001      127    25350 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx
--rw-r--r--   0     1001      127     9907 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/__init__.py
--rw-r--r--   0     1001      127      999 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/fuel_converters/__init__.py
--rw-r--r--   0     1001      127      191 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/README.md
--rw-r--r--   0     1001      127       15 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/link_points_idx_simple_corridor.csv
--rw-r--r--   0     1001      127     2279 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/speed_trace.csv
--rw-r--r--   0     1001      127      274 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/speed_trace_simple_corridor.csv
--rw-r--r--   0     1001      127      350 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/link_points_idx.csv
--rw-r--r--   0     1001      127      253 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/Default Demand.csv
--rw-r--r--   0     1001      127    67018 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/TimedPaths.csv
--rw-r--r--   0     1001      127  3119913 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/Taconite-NoBalloon.yaml
--rw-r--r--   0     1001      127      390 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/default_locations.csv
--rw-r--r--   0     1001      127     1153 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/links_test.yaml
--rw-r--r--   0     1001      127      136 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/network_charging_guidelines.csv
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/__init__.py
--rw-r--r--   0     1001      127  3128676 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/Taconite_v0.1.6.yaml
--rw-r--r--   0     1001      127      548 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv
--rw-r--r--   0     1001      127     3595 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/simple_corridor_network.yaml
--rw-r--r--   0     1001      127      214 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/simple_corridor_locations.csv
--rw-r--r--   0     1001      127  3192802 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/Taconite.yaml
--rw-r--r--   0     1001      127     2074 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/defaults.py
--rw-r--r--   0     1001      127     6896 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/rollout.py
--rw-r--r--   0     1001      127     3448 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/loaders/powertrain_components.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/loaders/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/user_interface.py
--rw-r--r--   0     1001      127     5693 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/sim_manager.py
--rw-r--r--   0     1001      127      603 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_consist.py
--rw-r--r--   0     1001      127      652 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_rail_vehicles.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_multi_obj_opt.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_fuel_grid.py
--rw-r--r--   0     1001      127     1279 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_fuel_conv.py
--rw-r--r--   0     1001      127     1019 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_utilities.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_objectives.py
--rw-r--r--   0     1001      127      747 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_generator.py
--rw-r--r--   0     1001      127     1533 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_locomotive.py
--rw-r--r--   0     1001      127      229 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_train_planner.py
--rw-r--r--   0     1001      127      874 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_edrive.py
--rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/__init__.py
--rw-r--r--   0     1001      127      675 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_consist_sim.py
--rw-r--r--   0     1001      127     2351 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_multi_obj_cal_and_val.py
--rw-r--r--   0     1001      127     1754 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_res.py
--rw-r--r--   0     1001      127      928 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_metric_calculator.py
--rw-r--r--   0     1001      127      386 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_train_simulation.py
--rw-r--r--   0     1001      127     7941 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/mock_resources.py
--rw-r--r--   0     1001      127      689 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_locomotive_simulation.py
--rw-r--r--   0     1001      127    29921 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/altrios_pyo3.pyi
--rw-r--r--   0     1001      127       91 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/optimization/multi_obj_opt.py
--rw-r--r--   0     1001      127       25 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/optimization/__init__.py
--rw-r--r--   0     1001      127    24477 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/optimization/cal_and_val.py
--rw-r--r--   0     1001      127     7492 2024-05-14 17:29:53.000000 altrios-0.2.2/README.md
--rw-r--r--   0     1001      127     1660 2024-05-14 17:29:53.000000 altrios-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 altrios-0.2.2/PKG-INFO
+-rw-r--r--   0     1001      127     1201 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/Cargo.toml
+-rw-r--r--   0     1001      127      784 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/README.md
+-rw-r--r--   0     1001      127     2475 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/combo_error.rs
+-rw-r--r--   0     1001      127    23033 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/consist_model.rs
+-rw-r--r--   0     1001      127     4145 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/consist_sim.rs
+-rw-r--r--   0     1001      127    12243 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/consist_utils.rs
+-rw-r--r--   0     1001      127     3330 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs
+-rw-r--r--   0     1001      127     3782 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/conventional_loco.rs
+-rw-r--r--   0     1001      127    12181 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs
+-rw-r--r--   0     1001      127    13669 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/loco_sim.rs
+-rw-r--r--   0     1001      127    40276 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/locomotive_model.rs
+-rw-r--r--   0     1001      127      991 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/mod.rs
+-rw-r--r--   0     1001      127      430 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.default.yaml
+-rw-r--r--   0     1001      127    15059 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs
+-rw-r--r--   0     1001      127     1034 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml
+-rw-r--r--   0     1001      127    13435 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs
+-rw-r--r--   0     1001      127      348 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/generator.default.yaml
+-rw-r--r--   0     1001      127    14503 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs
+-rw-r--r--   0     1001      127      213 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/mod.rs
+-rw-r--r--   0     1001      127      938 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs
+-rw-r--r--   0     1001      127     9907 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml
+-rw-r--r--   0     1001      127    30946 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs
+-rw-r--r--   0     1001      127      200 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/test.rs
+-rw-r--r--   0     1001      127     2790 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/locomotive/tests.rs
+-rw-r--r--   0     1001      127      752 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/mod.rs
+-rw-r--r--   0     1001      127     1039 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/consist/tests.rs
+-rw-r--r--   0     1001      127     1254 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/imports.rs
+-rw-r--r--   0     1001      127     1212 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/lib.rs
+-rw-r--r--   0     1001      127     1602 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/lin_search_hint.rs
+-rw-r--r--   0     1001      127     8028 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/macros.rs
+-rw-r--r--   0     1001      127      482 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/disp_imports.rs
+-rw-r--r--   0     1001      127     5431 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/disp_structs.rs
+-rw-r--r--   0     1001      127    11495 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/dispatch.rs
+-rw-r--r--   0     1001      127     2661 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs
+-rw-r--r--   0     1001      127    29031 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/est_times/mod.rs
+-rw-r--r--   0     1001      127     9721 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/est_times/update_times.rs
+-rw-r--r--   0     1001      127      281 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/mod.rs
+-rw-r--r--   0     1001      127    25666 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs
+-rw-r--r--   0     1001      127    36649 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/train_disp/free_path.rs
+-rw-r--r--   0     1001      127     9540 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/meet_pass/train_disp/mod.rs
+-rw-r--r--   0     1001      127     1969 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/prelude.rs
+-rw-r--r--   0     1001      127      255 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/pyo3.rs
+-rw-r--r--   0     1001      127     1039 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/si.rs
+-rw-r--r--   0     1001      127     2613 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/testing.rs
+-rw-r--r--   0     1001      127     2129 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/cat_power.rs
+-rw-r--r--   0     1001      127     4039 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/elev.rs
+-rw-r--r--   0     1001      127     4947 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/heading.rs
+-rw-r--r--   0     1001      127     4752 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/link_idx.rs
+-rw-r--r--   0     1001      127    23685 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/link_impl.rs
+-rw-r--r--   0     1001      127     1387 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/link_old.rs
+-rw-r--r--   0     1001      127     1900 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/location.rs
+-rw-r--r--   0     1001      127      246 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/locations.csv
+-rw-r--r--   0     1001      127      301 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/mod.rs
+-rw-r--r--   0     1001      127     4792 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/speed/speed_limit.rs
+-rw-r--r--   0     1001      127     3242 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/speed/speed_param.rs
+-rw-r--r--   0     1001      127     5971 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/speed/speed_set.rs
+-rw-r--r--   0     1001      127      120 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/link/speed.rs
+-rw-r--r--   0     1001      127      120 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/mod.rs
+-rw-r--r--   0     1001      127     6079 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/path_track/link_point.rs
+-rw-r--r--   0     1001      127      182 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/path_track/mod.rs
+-rw-r--r--   0     1001      127     2826 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/path_track/path_res_coeff.rs
+-rw-r--r--   0     1001      127    19995 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/path_track/path_tpc.rs
+-rw-r--r--   0     1001      127     7804 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/path_track/speed_point.rs
+-rw-r--r--   0     1001      127     3842 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/track/path_track/train_params.rs
+-rw-r--r--   0     1001      127     6268 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/braking_point.rs
+-rw-r--r--   0     1001      127     3503 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/friction_brakes.rs
+-rw-r--r--   0     1001      127      344 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/mod.rs
+-rw-r--r--   0     1001      127     3605 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/rail_vehicle.rs
+-rw-r--r--   0     1001      127     1124 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs
+-rw-r--r--   0     1001      127      324 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/bearing.rs
+-rw-r--r--   0     1001      127      438 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/davis_b.rs
+-rw-r--r--   0     1001      127       90 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/mod.rs
+-rw-r--r--   0     1001      127     4274 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/path_res.rs
+-rw-r--r--   0     1001      127      397 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/rolling.rs
+-rw-r--r--   0     1001      127      133 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/method/mod.rs
+-rw-r--r--   0     1001      127     2253 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/method/point.rs
+-rw-r--r--   0     1001      127     2758 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/method/strap.rs
+-rw-r--r--   0     1001      127     1780 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/resistance/mod.rs
+-rw-r--r--   0     1001      127    14039 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/set_speed_train_sim.rs
+-rw-r--r--   0     1001      127    25181 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/speed_limit_train_sim.rs
+-rw-r--r--   0     1001      127      443 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/test_rail_vehicles.csv
+-rw-r--r--   0     1001      127      182 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/timed_path.rs
+-rw-r--r--   0     1001      127    40645 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/train_config.rs
+-rw-r--r--   0     1001      127      338 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/train_imports.rs
+-rw-r--r--   0     1001      127     8339 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/train/train_state.rs
+-rw-r--r--   0     1001      127    10250 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/traits.rs
+-rw-r--r--   0     1001      127     2849 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/uc.rs
+-rw-r--r--   0     1001      127    13949 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     2455 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/utils/val_range.rs
+-rw-r--r--   0     1001      127     7292 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/src/validate.rs
+-rw-r--r--   0     1001      127      578 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/Cargo.toml
+-rw-r--r--   0     1001      127      707 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/README.md
+-rw-r--r--   0     1001      127    10749 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs
+-rw-r--r--   0     1001      127    12388 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs
+-rw-r--r--   0     1001      127     4551 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs
+-rw-r--r--   0     1001      127     2741 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs
+-rw-r--r--   0     1001      127      367 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/imports.rs
+-rw-r--r--   0     1001      127     1192 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/lib.rs
+-rw-r--r--   0     1001      127      571 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs
+-rw-r--r--   0     1001      127     3154 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/utilities.rs
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 altrios-0.2.3/rust/altrios-py/Cargo.toml
+-rw-r--r--   0     1001      127      586 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-py/README.md
+-rw-r--r--   0     1001      127     3080 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/altrios-py/src/lib.rs
+-rw-r--r--   0     1001      127    62818 2024-05-26 06:27:41.000000 altrios-0.2.3/rust/Cargo.lock
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 altrios-0.2.3/rust/Cargo.toml
+-rw-r--r--   0     1001      127     2197 2024-05-26 06:27:41.000000 altrios-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/loaders/__init__.py
+-rw-r--r--   0     1001      127     3448 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/loaders/powertrain_components.py
+-rw-r--r--   0     1001      127    10195 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/utilities.py
+-rw-r--r--   0     1001      127    16755 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/stringline.py
+-rw-r--r--   0     1001      127     1149 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/__init__.py
+-rw-r--r--   0     1001      127    41804 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/metric_calculator.py
+-rw-r--r--   0     1001      127     2074 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/defaults.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/objectives.py
+-rw-r--r--   0     1001      127    52841 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/output_12072022.csv
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/py.typed
+-rw-r--r--   0     1001      127    53858 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/train_planner.py
+-rw-r--r--   0     1001      127     6896 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/rollout.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/user_interface.py
+-rw-r--r--   0     1001      127      766 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/stringline_old.py
+-rw-r--r--   0     1001      127      386 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/plot.py
+-rw-r--r--   0     1001      127     5693 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/sim_manager.py
+-rw-r--r--   0     1001      127      111 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/__init__.py
+-rw-r--r--   0     1001      127     3410 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/set_speed_simple_corr_demo.py
+-rw-r--r--   0     1001      127     3903 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/set_speed_train_sim_demo.py
+-rw-r--r--   0     1001      127     4220 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/speed_limit_simple_corr_demo.py
+-rw-r--r--   0     1001      127     2357 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/conv_demo.py
+-rw-r--r--   0     1001      127      578 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/test_demos.py
+-rw-r--r--   0     1001      127     2377 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/bel_demo.py
+-rw-r--r--   0     1001      127     1006 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/version_migration_demo.py
+-rw-r--r--   0     1001      127     3488 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/rollout_demo.py
+-rw-r--r--   0     1001      127      278 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/demo_logging.py
+-rw-r--r--   0     1001      127     6086 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/speed_limit_train_sim_demo.py
+-rw-r--r--   0     1001      127     5592 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/demos/sim_manager_demo.py
+-rw-r--r--   0     1001      127      994 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv
+-rw-r--r--   0     1001      127     1616 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv
+-rw-r--r--   0     1001      127   128287 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv
+-rw-r--r--   0     1001      127    10562 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv
+-rw-r--r--   0     1001      127     2025 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv
+-rw-r--r--   0     1001      127  1237826 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv
+-rw-r--r--   0     1001      127      695 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/Default Demand StoBar.csv
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/__init__.py
+-rw-r--r--   0     1001      127  3128676 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/Taconite_v0.1.6.yaml
+-rw-r--r--   0     1001      127      136 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/network_charging_guidelines.csv
+-rw-r--r--   0     1001      127  3192802 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/Taconite.yaml
+-rw-r--r--   0     1001      127     1153 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/links_test.yaml
+-rw-r--r--   0     1001      127      214 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/simple_corridor_locations.csv
+-rw-r--r--   0     1001      127      390 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/default_locations.csv
+-rw-r--r--   0     1001      127  3119913 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/Taconite-NoBalloon.yaml
+-rw-r--r--   0     1001      127      548 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv
+-rw-r--r--   0     1001      127     3595 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/networks/simple_corridor_network.yaml
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/powertrains/reversible_energy_storages/__init__.py
+-rw-r--r--   0     1001      127     9907 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml
+-rw-r--r--   0     1001      127    25350 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/powertrains/__init__.py
+-rw-r--r--   0     1001      127      999 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/powertrains/fuel_converters/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/__init__.py
+-rw-r--r--   0     1001      127      511 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/Manifest.yaml
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/__init__.py
+-rw-r--r--   0     1001      127      641 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/rail_vehicles.csv
+-rw-r--r--   0     1001      127      492 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/Unit_Empty.yaml
+-rw-r--r--   0     1001      127      496 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/Manifest_Empty.yaml
+-rw-r--r--   0     1001      127      498 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/Intermodal_Empty.yaml
+-rw-r--r--   0     1001      127      501 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/Unit.yaml
+-rw-r--r--   0     1001      127      492 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/rolling_stock/Intermodal.yaml
+-rw-r--r--   0     1001      127      253 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/Default Demand.csv
+-rw-r--r--   0     1001      127      191 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/demo_data/README.md
+-rw-r--r--   0     1001      127       15 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/demo_data/link_points_idx_simple_corridor.csv
+-rw-r--r--   0     1001      127      350 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/demo_data/link_points_idx.csv
+-rw-r--r--   0     1001      127      274 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/demo_data/speed_trace_simple_corridor.csv
+-rw-r--r--   0     1001      127     2279 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/demo_data/speed_trace.csv
+-rw-r--r--   0     1001      127       50 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/tpc_input_example.csv
+-rw-r--r--   0     1001      127      568 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/trains/train_res_temp.yaml
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/trains/__init__.py
+-rw-r--r--   0     1001      127    67018 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/TimedPaths.csv
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/resources/powertrain_model_input_example.csv
+-rw-r--r--   0     1001      127    29921 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/altrios_pyo3.pyi
+-rw-r--r--   0     1001      127       25 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/optimization/__init__.py
+-rw-r--r--   0     1001      127       91 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/optimization/multi_obj_opt.py
+-rw-r--r--   0     1001      127    24477 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/optimization/cal_and_val.py
+-rw-r--r--   0     1001      127     1533 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_locomotive.py
+-rw-r--r--   0     1001      127     1019 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_utilities.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/__init__.py
+-rw-r--r--   0     1001      127      675 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_consist_sim.py
+-rw-r--r--   0     1001      127      603 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_consist.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_fuel_grid.py
+-rw-r--r--   0     1001      127     1754 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_powertrain_res.py
+-rw-r--r--   0     1001      127      386 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_train_simulation.py
+-rw-r--r--   0     1001      127     1279 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_powertrain_fuel_conv.py
+-rw-r--r--   0     1001      127      928 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_metric_calculator.py
+-rw-r--r--   0     1001      127      874 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_powertrain_edrive.py
+-rw-r--r--   0     1001      127      689 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_locomotive_simulation.py
+-rw-r--r--   0     1001      127      652 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_rail_vehicles.py
+-rw-r--r--   0     1001      127      229 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_train_planner.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_multi_obj_opt.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_objectives.py
+-rw-r--r--   0     1001      127      747 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_powertrain_generator.py
+-rw-r--r--   0     1001      127     7941 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/mock_resources.py
+-rw-r--r--   0     1001      127     2351 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/tests/test_multi_obj_cal_and_val.py
+-rw-r--r--   0     1001      127        0 2024-05-26 06:27:41.000000 altrios-0.2.3/python/altrios/fuel_grid.py
+-rw-r--r--   0     1001      127     7461 2024-05-26 06:27:41.000000 altrios-0.2.3/README.md
+-rw-r--r--   0     1001      127     1660 2024-05-26 06:27:41.000000 altrios-0.2.3/LICENSE.md
+-rw-r--r--   0        0        0     9071 1970-01-01 00:00:00.000000 altrios-0.2.3/PKG-INFO
```

### Comparing `altrios-0.2.2/rust/altrios-core/Cargo.toml` & `altrios-0.2.3/rust/altrios-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/README.md` & `altrios-0.2.3/rust/altrios-core/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/combo_error.rs` & `altrios-0.2.3/rust/altrios-core/src/combo_error.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/consist_model.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/consist_model.rs`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,18 @@
     n_res_equipped: Option<u8>,
 }
 
 impl SerdeAPI for Consist {
     fn init(&mut self) -> anyhow::Result<()> {
         self.check_mass_consistent()?;
         self.set_pwr_dyn_brake_max();
+        self.loco_vec.init()?;
+        self.pdct.init()?;
+        self.state.init()?;
+        self.history.init()?;
         Ok(())
     }
 }
 
 impl Consist {
     pub fn new(
         loco_vec: Vec<Locomotive>,
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/consist_sim.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/consist_sim.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use serde::{Deserialize, Serialize};
 
 use crate::consist::locomotive::loco_sim::PowerTrace;
 use crate::consist::Consist;
 use crate::consist::LocoTrait;
 use crate::imports::*;
 
-#[derive(Clone, Debug, Deserialize, Serialize, PartialEq, SerdeAPI)]
+#[derive(Clone, Debug, Deserialize, Serialize, PartialEq)]
 #[altrios_api(
     #[new]
     fn __new__(consist: Consist, power_trace: PowerTrace, save_interval: Option<usize>) -> Self {
         Self::new(consist, power_trace, save_interval)
     }
 
     #[pyo3(name = "walk")]
@@ -114,14 +114,22 @@
     ) -> anyhow::Result<()> {
         self.loco_con
             .solve_energy_consumption(pwr_out_req, dt, Some(true))?;
         Ok(())
     }
 }
 
+impl SerdeAPI for ConsistSimulation {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.loco_con.init()?;
+        self.power_trace.init()?;
+        Ok(())
+    }
+}
+
 impl Default for ConsistSimulation {
     fn default() -> Self {
         Self::new(Consist::default(), PowerTrace::default(), Some(1))
     }
 }
 
 #[cfg(test)]
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/consist_utils.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/consist_utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,25 @@
         unimplemented!();
     }
     /// Get energy loss in components
     fn get_energy_loss(&self) -> si::Energy;
 }
 
 #[altrios_api]
-#[derive(Default, Serialize, Deserialize, Clone, PartialEq, SerdeAPI)]
+#[derive(Default, Serialize, Deserialize, Clone, PartialEq)]
 /// Wrapper struct for `Vec<Locomotive>` to expose various methods to Python.
 pub struct Pyo3VecLocoWrapper(pub Vec<Locomotive>);
 
+impl SerdeAPI for Pyo3VecLocoWrapper {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.0.iter_mut().try_for_each(|l| l.init())?;
+        Ok(())
+    }
+}
+
 pub trait SolvePower {
     /// Returns vector of locomotive tractive powers during positive traction events
     fn solve_positive_traction(
         &mut self,
         loco_vec: &[Locomotive],
         state: &ConsistState,
     ) -> anyhow::Result<Vec<si::Power>>;
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use super::powertrain::electric_drivetrain::ElectricDrivetrain;
 use super::powertrain::reversible_energy_storage::ReversibleEnergyStorage;
 use super::powertrain::ElectricMachine;
 use super::LocoTrait;
 use crate::imports::*;
 
-#[derive(Default, Clone, Debug, PartialEq, Serialize, Deserialize, HistoryMethods, SerdeAPI)]
+#[derive(Default, Clone, Debug, PartialEq, Serialize, Deserialize, HistoryMethods)]
 #[altrios_api(
     #[new]
     fn __new__(
         res: ReversibleEnergyStorage,
         edrv: ElectricDrivetrain,
     ) -> Self {
         Self { res, edrv }
@@ -60,14 +60,22 @@
                 dt,
             )?;
         }
         Ok(())
     }
 }
 
+impl SerdeAPI for BatteryElectricLoco {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.res.init()?;
+        self.edrv.init()?;
+        Ok(())
+    }
+}
+
 impl LocoTrait for BatteryElectricLoco {
     fn set_cur_pwr_max_out(
         &mut self,
         pwr_aux: Option<si::Power>,
         dt: si::Time,
     ) -> anyhow::Result<()> {
         // TODO: proposed interface location to feed in the catenary
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/conventional_loco.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/conventional_loco.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use super::powertrain::electric_drivetrain::ElectricDrivetrain;
 use super::powertrain::fuel_converter::FuelConverter;
 use super::powertrain::generator::Generator;
 use super::powertrain::ElectricMachine;
 use super::LocoTrait;
 use crate::imports::*;
 
-#[derive(Default, Clone, Debug, PartialEq, Serialize, Deserialize, HistoryMethods, SerdeAPI)]
+#[derive(Default, Clone, Debug, PartialEq, Serialize, Deserialize, HistoryMethods)]
 #[altrios_api(
     #[new]
     pub fn __new__(
         fuel_converter: FuelConverter,
         generator: Generator,
         electric_drivetrain: ElectricDrivetrain,
     ) -> Self {
@@ -80,14 +80,23 @@
             engine_on,
             assert_limits,
         )?;
         Ok(())
     }
 }
 
+impl SerdeAPI for ConventionalLoco {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.fc.init()?;
+        self.gen.init()?;
+        self.edrv.init()?;
+        Ok(())
+    }
+}
+
 impl LocoTrait for ConventionalLoco {
     /// returns current max power, current max power rate, and current max regen
     /// power that can be absorbed by the RES/battery
     fn set_cur_pwr_max_out(
         &mut self,
         pwr_aux: Option<si::Power>,
         dt: si::Time,
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,23 @@
     /// time step needed for solving for optimal fuel/res split.
     /// should not be public!
     dt: si::Time,
     /// step counter for gss_interval check
     i: usize,
 }
 
-impl SerdeAPI for HybridLoco {}
+impl SerdeAPI for HybridLoco {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.fc.init()?;
+        self.gen.init()?;
+        self.res.init()?;
+        self.edrv.init()?;
+        Ok(())
+    }
+}
 
 impl Default for HybridLoco {
     fn default() -> Self {
         Self {
             fc: FuelConverter::default(),
             gen: Generator::default(),
             res: ReversibleEnergyStorage::default(),
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/loco_sim.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/loco_sim.rs`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
     #[pyo3(name = "trim_failed_steps")]
     fn trim_failed_steps_py(&mut self) -> anyhow::Result<()> {
         self.trim_failed_steps()?;
         Ok(())
     }
 )]
-#[derive(Clone, Debug, Deserialize, Serialize, PartialEq, SerdeAPI)]
+#[derive(Clone, Debug, Deserialize, Serialize, PartialEq)]
 /// Struct for simulating operation of a standalone locomotive.
 pub struct LocomotiveSimulation {
     pub loco_unit: Locomotive,
     pub power_trace: PowerTrace,
     pub i: usize,
 }
 
@@ -279,14 +279,22 @@
     ) -> anyhow::Result<()> {
         self.loco_unit
             .solve_energy_consumption(pwr_out_req, dt, engine_on)?;
         Ok(())
     }
 }
 
+impl SerdeAPI for LocomotiveSimulation {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.loco_unit.init()?;
+        self.power_trace.init()?;
+        Ok(())
+    }
+}
+
 impl Default for LocomotiveSimulation {
     fn default() -> Self {
         let power_trace = PowerTrace::default();
         let loco_unit = Locomotive::default();
         Self::new(loco_unit, power_trace, None)
     }
 }
@@ -295,17 +303,23 @@
     #[pyo3(name="walk")]
     /// Exposes `walk` to Python.
     fn walk_py(&mut self, b_parallelize: Option<bool>) -> anyhow::Result<()> {
         let b_par = b_parallelize.unwrap_or(false);
         self.walk(b_par)
     }
 )]
-#[derive(Clone, Debug, Serialize, Deserialize, SerdeAPI)]
+#[derive(Clone, Debug, Serialize, Deserialize)]
 pub struct LocomotiveSimulationVec(pub Vec<LocomotiveSimulation>);
 
+impl SerdeAPI for LocomotiveSimulationVec {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.0.iter_mut().try_for_each(|l| l.init())?;
+        Ok(())
+    }
+}
 impl Default for LocomotiveSimulationVec {
     fn default() -> Self {
         Self(vec![LocomotiveSimulation::default(); 3])
     }
 }
 
 impl LocomotiveSimulationVec {
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/locomotive_model.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/locomotive_model.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 use super::*;
 
-#[derive(Clone, Debug, Serialize, Deserialize, PartialEq, SerdeAPI)]
+#[derive(Clone, Debug, Serialize, Deserialize, PartialEq)]
 pub enum PowertrainType {
     ConventionalLoco(ConventionalLoco),
     HybridLoco(Box<HybridLoco>),
     BatteryElectricLoco(BatteryElectricLoco),
     DummyLoco(DummyLoco),
 }
 
+impl SerdeAPI for PowertrainType {
+    fn init(&mut self) -> anyhow::Result<()> {
+        match self {
+            Self::ConventionalLoco(l) => l.init()?,
+            Self::HybridLoco(l) => l.init()?,
+            Self::BatteryElectricLoco(l) => l.init()?,
+            Self::DummyLoco(_) => {}
+        };
+        Ok(())
+    }
+}
+
 impl LocoTrait for PowertrainType {
     fn set_cur_pwr_max_out(
         &mut self,
         pwr_aux: Option<si::Power>,
         dt: si::Time,
     ) -> anyhow::Result<()> {
         match self {
@@ -555,14 +567,15 @@
         loco
     }
 }
 
 impl SerdeAPI for Locomotive {
     fn init(&mut self) -> anyhow::Result<()> {
         self.check_mass_consistent()?;
+        self.loco_type.init()?;
         Ok(())
     }
 }
 
 impl Mass for Locomotive {
     fn mass(&self) -> anyhow::Result<Option<si::Mass>> {
         self.check_mass_consistent()?;
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/mod.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     }
 
     #[setter("__eta_range")]
     fn set_eta_range_py(&mut self, eta_range: f64) -> anyhow::Result<()> {
         Ok(self.set_eta_range(eta_range).map_err(PyValueError::new_err)?)
     }
 )]
-#[derive(Deserialize, Serialize, Debug, Clone, PartialEq, HistoryMethods, SerdeAPI)]
+#[derive(Deserialize, Serialize, Debug, Clone, PartialEq, HistoryMethods)]
 /// Struct for modeling electric drivetrain.  This includes power electronics, motor, axle ...
 /// everything involved in converting high voltage electrical power to force exerted by the wheel on the track.  
 pub struct ElectricDrivetrain {
     #[serde(default)]
     /// struct for tracking current state
     pub state: ElectricDrivetrainState,
     /// Shaft output power fraction array at which efficiencies are evaluated.
@@ -230,14 +230,21 @@
 
 // failed attempt at making path to default platform independent
 // const EDRV_DEFAULT_PATH_STR: &'static str = include_str!(concat!(
 //     env!("CARGO_MANIFEST_DIR"),
 //     "/src/consist/locomotive/powertrain/electric_drivetrain.default.yaml"
 // ));
 
+impl SerdeAPI for ElectricDrivetrain {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.state.init()?;
+        Ok(())
+    }
+}
+
 impl Default for ElectricDrivetrain {
     fn default() -> Self {
         // let file_contents = include_str!(EDRV_DEFAULT_PATH_STR);
         let file_contents = include_str!("electric_drivetrain.default.yaml");
         serde_yaml::from_str::<ElectricDrivetrain>(file_contents).unwrap()
     }
 }
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         serde_yaml::from_str::<FuelConverter>(file_contents).unwrap()
     }
 }
 
 impl SerdeAPI for FuelConverter {
     fn init(&mut self) -> anyhow::Result<()> {
         self.check_mass_consistent()?;
+        self.state.init()?;
         Ok(())
     }
 }
 
 impl Mass for FuelConverter {
     fn mass(&self) -> anyhow::Result<Option<si::Mass>> {
         self.check_mass_consistent()?;
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     #[serde(default)]
     pub history: GeneratorStateHistoryVec,
 }
 
 impl SerdeAPI for Generator {
     fn init(&mut self) -> anyhow::Result<()> {
         self.check_mass_consistent()?;
+        self.state.init()?;
         Ok(())
     }
 }
 
 impl Mass for Generator {
     fn mass(&self) -> anyhow::Result<Option<si::Mass>> {
         self.check_mass_consistent()?;
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,15 @@
         Ok(())
     }
 }
 
 impl SerdeAPI for ReversibleEnergyStorage {
     fn init(&mut self) -> anyhow::Result<()> {
         self.check_mass_consistent()?;
+        self.state.init()?;
         Ok(())
     }
 }
 
 #[allow(unused)]
 impl ReversibleEnergyStorage {
     #[allow(clippy::too_many_arguments)]
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/tests.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/locomotive/tests.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/mod.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/consist/tests.rs` & `altrios-0.2.3/rust/altrios-core/src/consist/tests.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/imports.rs` & `altrios-0.2.3/rust/altrios-core/src/imports.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/lib.rs` & `altrios-0.2.3/rust/altrios-core/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 // TODO: uncomment when docs are somewhat mature to check for missing docs
 // #![warn(missing_docs)]
 // #![warn(missing_docs_in_private_items)]
 
 //! Crate containing models for second-by-second fuel and energy consumption of simulation
 //! of locomotive consists comprising collections of individual locomotives, which comprise
 //! various powertrain components (engine, generator/alternator, battery, and electric drivetrain)
-//! -- all connected to a detailed train model.  
+//! -- all connected to a detailed train model including drag, grade, curvature, bearing, and
+//! rolling resistances.  
 //!
 //! # Helpful Tips
 //! Every struct in this crate implements methods for serializing/deserializing itself to/from a
 //! handful of standard data formats as strings or file read/write operations using
 //! [traits::SerdeAPI].   
 //!
 //! # Features:
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/lin_search_hint.rs` & `altrios-0.2.3/rust/altrios-core/src/lin_search_hint.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/macros.rs` & `altrios-0.2.3/rust/altrios-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/disp_structs.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/disp_structs.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/dispatch.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/dispatch.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/mod.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/est_times/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/update_times.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/est_times/update_times.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/free_path.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/train_disp/free_path.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/mod.rs` & `altrios-0.2.3/rust/altrios-core/src/meet_pass/train_disp/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/prelude.rs` & `altrios-0.2.3/rust/altrios-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/si.rs` & `altrios-0.2.3/rust/altrios-core/src/si.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/testing.rs` & `altrios-0.2.3/rust/altrios-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/cat_power.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/cat_power.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/elev.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/elev.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/heading.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/heading.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/link_idx.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/link_idx.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/link_impl.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/link_impl.rs`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 #[derive(Debug, Default, Clone, Serialize, Deserialize, PartialEq, SerdeAPI)]
 /// An arbitrary unit of single track that does not include turnouts
 #[altrios_api()]
 pub struct Link {
     /// Index of current link
     pub idx_curr: LinkIdx,
-    /// Index of adjacent link in reverse direction
+    /// Index of current link in reverse direction
     pub idx_flip: LinkIdx,
     /// see [EstTime::idx_next]
     pub idx_next: LinkIdx,
     /// see [EstTime::idx_next_alt]  
     /// if it does not exist, it should be `LinkIdx{idx: 0}`
     pub idx_next_alt: LinkIdx,
     /// see [EstTime::idx_prev]
@@ -374,15 +374,15 @@
         if self.len() < 2 {
             errors.push(anyhow!(
                 "There must be at least two links (one physical and one dummy)!"
             ));
             return Err(errors);
         }
         validate_slice_fake(&mut errors, &self[..1], "Link");
-        validate_slice_real_shift(&mut errors, &self[1..], "Link", 1);
+        validate_slice_real_shift(&mut errors, &self[1..], "Link", 0);
         early_err!(errors, "Links");
 
         for (idx, link) in self.iter().enumerate().skip(1) {
             // Validate flip and curr
             if link.idx_curr.idx() != idx {
                 errors.push(anyhow!(
                     "Link idx {} is not equal to index in vector {}!",
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/link_old.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/link_old.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/location.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/location.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_limit.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/speed/speed_limit.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_param.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/speed/speed_param.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_set.rs` & `altrios-0.2.3/rust/altrios-core/src/track/link/speed/speed_set.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/path_track/link_point.rs` & `altrios-0.2.3/rust/altrios-core/src/track/path_track/link_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/path_track/path_res_coeff.rs` & `altrios-0.2.3/rust/altrios-core/src/track/path_track/path_res_coeff.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/path_track/path_tpc.rs` & `altrios-0.2.3/rust/altrios-core/src/track/path_track/path_tpc.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/path_track/speed_point.rs` & `altrios-0.2.3/rust/altrios-core/src/track/path_track/speed_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/track/path_track/train_params.rs` & `altrios-0.2.3/rust/altrios-core/src/track/path_track/train_params.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/braking_point.rs` & `altrios-0.2.3/rust/altrios-core/src/train/braking_point.rs`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,21 @@
                     train_state.offset = bp_curr.offset;
                     train_state.speed = bp_curr.speed_limit;
                     train_res.update_res(&mut train_state, path_tpc, &Dir::Bwd)?;
 
                     ensure!(
                         fric_brake.force_max + train_state.res_net() > si::Force::ZERO,
                         format!(
-                            "{}\n{}\n{}",
+                            "{}\n{}\n{}\n{}",
                             format_dbg!(
                                 fric_brake.force_max + train_state.res_net() > si::Force::ZERO
                             ),
                             format_dbg!(fric_brake.force_max),
                             format_dbg!(train_state.res_net()),
+                            format_dbg!(train_state.res_grade),
                         )
                     );
                     let vel_change = train_state.dt
                         * (fric_brake.force_max + train_state.res_net())
                         / train_state.mass_static;
 
                     // Exit after adding a couple of points if the next braking curve point will exceed the speed limit
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/friction_brakes.rs` & `altrios-0.2.3/rust/altrios-core/src/train/friction_brakes.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/rail_vehicle.rs` & `altrios-0.2.3/rust/altrios-core/src/train/rail_vehicle.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs` & `altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/path_res.rs` & `altrios-0.2.3/rust/altrios-core/src/train/resistance/kind/path_res.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/resistance/method/point.rs` & `altrios-0.2.3/rust/altrios-core/src/train/resistance/method/point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/resistance/method/strap.rs` & `altrios-0.2.3/rust/altrios-core/src/train/resistance/method/strap.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/resistance/mod.rs` & `altrios-0.2.3/rust/altrios-core/src/train/resistance/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/set_speed_train_sim.rs` & `altrios-0.2.3/rust/altrios-core/src/train/set_speed_train_sim.rs`

 * *Files 5% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
     #[pyo3(name = "trim_failed_steps")]
     fn trim_failed_steps_py(&mut self) -> anyhow::Result<()> {
         self.trim_failed_steps()?;
         Ok(())
     }
 )]
-#[derive(Clone, Debug, Serialize, Deserialize, SerdeAPI)]
+#[derive(Clone, Debug, Serialize, Deserialize)]
 /// Train simulation in which speed is prescribed
 pub struct SetSpeedTrainSim {
     pub loco_con: Consist,
     pub state: TrainState,
     pub speed_trace: SpeedTrace,
     #[api(skip_get, skip_set)]
     /// train resistance calculation
@@ -397,14 +397,26 @@
             self.state.energy_whl_out_pos += self.state.pwr_whl_out * dt;
         } else {
             self.state.energy_whl_out_neg -= self.state.pwr_whl_out * dt;
         }
     }
 }
 
+impl SerdeAPI for SetSpeedTrainSim {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.loco_con.init()?;
+        self.speed_trace.init()?;
+        self.train_res.init()?;
+        self.path_tpc.init()?;
+        self.state.init()?;
+        self.history.init()?;
+        Ok(())
+    }
+}
+
 impl Default for SetSpeedTrainSim {
     fn default() -> Self {
         Self {
             loco_con: Consist::default(),
             state: TrainState::valid(),
             train_res: TrainRes::valid(),
             path_tpc: PathTpc::valid(),
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/speed_limit_train_sim.rs` & `altrios-0.2.3/rust/altrios-core/src/train/speed_limit_train_sim.rs`

 * *Files 6% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                 let tp = timed_path.extract::<Vec<LinkIdxTime>>().map_err(|_| anyhow!("{}", format_dbg!()))?;
                 TimedLinkPath(tp)
             }
         };
         self.walk_timed_path(&network, timed_path)
     }
 )]
-#[derive(Clone, Debug, Serialize, Deserialize, PartialEq, SerdeAPI)]
+#[derive(Clone, Debug, Serialize, Deserialize, PartialEq)]
 /// Train simulation in which speed is allowed to vary according to train capabilities and speed
 /// limit
 pub struct SpeedLimitTrainSim {
     #[api(skip_set)]
     pub train_id: String,
     pub origs: Vec<Location>,
     pub dests: Vec<Location>,
@@ -343,14 +343,15 @@
             bail!("Timed path cannot be empty!");
         }
 
         self.save_state();
         let mut idx_prev = 0;
         while idx_prev != timed_path.len() - 1 {
             let mut idx_next = idx_prev + 1;
+            log::debug!("Solving idx: {}", idx_next);
             while idx_next + 1 < timed_path.len() - 1 && timed_path[idx_next].time < self.state.time
             {
                 idx_next += 1;
             }
             let time_extend = timed_path[idx_next - 1].time;
             self.extend_path(
                 network,
@@ -374,25 +375,27 @@
     /// - inertia
     /// - target acceleration
     pub fn solve_required_pwr(&mut self) -> anyhow::Result<()> {
         let res_net = self.state.res_net();
 
         // Verify that train can slow down
         // TODO: figure out if dynamic braking needs to be separately accounted for here
-        if self.fric_brake.force_max + res_net <= si::Force::ZERO {
-            bail!(
-                "Train {} does not have sufficient braking to slow down at time{:?}.
-            Fric brake force = {:?}.
-            Net resistance = {:?}",
-                self.train_id,
-                self.state.time,
-                self.fric_brake.force_max,
-                res_net
-            );
-        }
+
+        ensure!(
+            self.fric_brake.force_max + self.state.res_net() > si::Force::ZERO,
+            format!(
+                "Insufficient braking force.\n{}\n{}\n{}\n{}\n{}\n{}",
+                format_dbg!(self.fric_brake.force_max + self.state.res_net() > si::Force::ZERO),
+                format_dbg!(self.fric_brake.force_max),
+                format_dbg!(self.state.res_net()),
+                format_dbg!(self.state.res_grade),
+                format_dbg!(self.state.grade_front),
+                format_dbg!(self.state.grade_back),
+            )
+        );
 
         // TODO: Validate that this makes sense considering friction brakes
         let (speed_limit, speed_target) = self.braking_points.calc_speeds(
             self.state.offset,
             self.state.speed,
             self.fric_brake.ramp_up_time * self.fric_brake.ramp_up_coeff,
         );
@@ -427,21 +430,21 @@
         // maximum achievable positive tractive force
         let f_pos_max = self
             .loco_con
             .force_max()?
             .min(pwr_pos_max / speed_target.min(v_max));
         // Verify that train has sufficient power to move
         if self.state.speed < uc::MPH * 0.1 && f_pos_max <= res_net {
+            log::error!("{}", format_dbg!(self.path_tpc));
             bail!(
                 "{}\nTrain does not have sufficient power to move!\nforce_max={:?},\nres_net={:?},\ntrain_state={:?}", // ,\nlink={:?}
                 format_dbg!(),
                 f_pos_max,
                 res_net,
                 self.state,
-                // self.path_tpc
             );
         }
 
         self.fric_brake.set_cur_force_max_out(self.state.dt)?;
 
         // Transition speed between force and power limited negative traction
         let v_neg_trac_lim: si::Velocity =
@@ -578,14 +581,29 @@
             &self.fric_brake,
             &self.train_res,
             &self.path_tpc,
         )
     }
 }
 
+impl SerdeAPI for SpeedLimitTrainSim {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.origs.init()?;
+        self.dests.init()?;
+        self.loco_con.init()?;
+        self.state.init()?;
+        self.train_res.init()?;
+        self.path_tpc.init()?;
+        self.braking_points.init()?;
+        self.fric_brake.init()?;
+        self.history.init()?;
+        Ok(())
+    }
+}
+
 impl Default for SpeedLimitTrainSim {
     fn default() -> Self {
         let mut slts = Self {
             train_id: Default::default(),
             origs: Default::default(),
             dests: Default::default(),
             loco_con: Default::default(),
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/train_config.rs` & `altrios-0.2.3/rust/altrios-core/src/train/train_config.rs`

 * *Files 0% similar despite different names*

```diff
@@ -990,15 +990,15 @@
     }
 
     #[pyo3(name = "set_save_interval")]
     pub fn set_save_interval_py(&mut self, save_interval: Option<usize>) {
         self.set_save_interval(save_interval);
     }
 )]
-#[derive(Default, Clone, Debug, Serialize, Deserialize, PartialEq, SerdeAPI)]
+#[derive(Default, Clone, Debug, Serialize, Deserialize, PartialEq)]
 pub struct SpeedLimitTrainSimVec(pub Vec<SpeedLimitTrainSim>);
 
 impl SpeedLimitTrainSimVec {
     pub fn get_energy_fuel(&self, annualize: bool) -> si::Energy {
         self.0
             .iter()
             .map(|sim| sim.get_energy_fuel(annualize))
@@ -1040,14 +1040,21 @@
     pub fn set_save_interval(&mut self, save_interval: Option<usize>) {
         self.0
             .iter_mut()
             .for_each(|slts| slts.set_save_interval(save_interval));
     }
 }
 
+impl SerdeAPI for SpeedLimitTrainSimVec {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.0.iter_mut().try_for_each(|ts| ts.init())?;
+        Ok(())
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::train::rail_vehicle::import_rail_vehicles;
 
     #[test]
     fn test_make_train_params() {
```

### Comparing `altrios-0.2.2/rust/altrios-core/src/train/train_state.rs` & `altrios-0.2.3/rust/altrios-core/src/train/train_state.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/traits.rs` & `altrios-0.2.3/rust/altrios-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/uc.rs` & `altrios-0.2.3/rust/altrios-core/src/uc.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/utils/mod.rs` & `altrios-0.2.3/rust/altrios-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/utils/val_range.rs` & `altrios-0.2.3/rust/altrios-core/src/utils/val_range.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/src/validate.rs` & `altrios-0.2.3/rust/altrios-core/src/validate.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/Cargo.toml` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/README.md` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,28 @@
         .collect::<Vec<_>>();
     let first_field = &field_names[0];
     let vec_fields = fields
         .iter()
         .map(|f| {
             let ident = f.ident.as_ref().unwrap();
             let ty = &f.ty;
+            let doc_attrs = &f
+                .attrs
+                .iter()
+                .filter(|attr| {
+                    if attr.path.is_ident("doc") {
+                        attr.parse_meta()
+                            .is_ok_and(|meta| matches!(meta, syn::Meta::NameValue(_)))
+                    } else {
+                        false
+                    }
+                })
+                .collect::<Vec<&syn::Attribute>>();
             quote! {
+                #(#doc_attrs)*
                 pub #ident: Vec<#ty>,
             }
         })
         .concat();
     let vec_new = fields
         .iter()
         .map(|f| {
```

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/lib.rs` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/utilities.rs` & `altrios-0.2.3/rust/altrios-core/altrios-proc-macros/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-py/Cargo.toml` & `altrios-0.2.3/rust/altrios-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-py/README.md` & `altrios-0.2.3/rust/altrios-py/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/altrios-py/src/lib.rs` & `altrios-0.2.3/rust/altrios-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/rust/Cargo.lock` & `altrios-0.2.3/rust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.3"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
+ "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.1"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea5d730647d4fadd988536d06fecce94b7b4f2a7efdae548f1cf4b63205518ab"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "altrios-core"
 version = "0.2.2"
 dependencies = [
  "altrios-proc-macros",
  "anyhow",
@@ -112,32 +113,32 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.75"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4668cab20f66d8d020e1fbc0ebe47217433c1b6c8f2040faf858554e394ace6"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "arc-swap"
-version = "1.6.0"
+version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "argmin"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3406b1667cb225f6a0242413b95da764ba118a859bef79f1aacf58d5c84d6511"
 dependencies = [
@@ -157,17 +158,17 @@
  "slog-json",
  "slog-term",
  "thiserror",
 ]
 
 [[package]]
 name = "argminmax"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "202108b46429b765ef483f8a24d5c46f48c14acfdacc086dd4ab6dddf6bcdbd2"
+checksum = "52424b59d69d69d5056d508b260553afd91c57e21849579cd1f50ee8b8b88eaa"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "array-init-cursor"
 version = "0.2.0"
@@ -211,54 +212,43 @@
  "simdutf8",
  "strength_reduce",
  "zstd",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.73"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc00ceb34980c03614e35a3a4e218276a0a824e911d07651cd0d858a51e8c0f0"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi",
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -272,227 +262,219 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "bitflags"
-version = "2.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4682ae6287fcf752ecaabbfcc7b6f9b72aa33933dc23a554d853aea8eea8635"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "374d28ec25809ee0e23827c2ab573d729e293f281dfe393500e7ad618baa61c6"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "965ab7eb5f8f97d2a083c799f3a1b994fc397b2fe2da5d1da1626ce15a39f2b1"
+checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
  "serde",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
+checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
+checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "comfy-table"
-version = "7.0.1"
+version = "7.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ab77dbd8adecaf3f0db40581631b995f312a8a5ae3aa9993188bb8f23d83a5b"
+checksum = "b34115915337defe99b2aff5c2ce6771e5fbc4079f4b506301f5cf394c8452f7"
 dependencies = [
  "crossterm",
  "strum",
- "strum_macros 0.24.3",
+ "strum_macros 0.26.2",
  "unicode-width",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.8"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
- "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.15"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if",
  "crossbeam-utils",
- "memoffset",
- "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.16"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
-dependencies = [
- "cfg-if",
-]
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "crossterm"
-version = "0.26.1"
+version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a84cda67535339806297f1b331d6dd6320470d2a0fe65381e79ee9e156dd3d13"
+checksum = "f476fe445d41c9e991fd07515a6f463074b782242ccf4a5b7b1d1012e70824df"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "crossterm_winapi",
  "libc",
- "mio",
  "parking_lot",
- "signal-hook",
- "signal-hook-mio",
  "winapi",
 ]
 
 [[package]]
 name = "crossterm_winapi"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acdd7c62a3665c7f6830a51635d9ac9b23ed385797f70a83bb8bafe9c572ab2b"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "csv"
-version = "1.2.2"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "626ae34994d3d8d668f4269922248239db4ae42d538b14c398b74a52208e8086"
+checksum = "ac574ff4d437a7b5ad237ef331c17ccca63c46479e5b5453eb8e10bb99a759fe"
 dependencies = [
  "csv-core",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "csv-core"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
+checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "deranged"
-version = "0.3.8"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2696e8a945f658fd14dc3b87242e6b80cd0f36ff04ea560fa39082368847946"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
+dependencies = [
+ "powerfmt",
+]
 
 [[package]]
 name = "directories"
 version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a49173b84e034382284f27f1af4dcbbd231ffa358c0fe316541a7337f376a35"
 dependencies = [
@@ -540,164 +522,164 @@
 dependencies = [
  "heck",
  "proc-macro-error",
 ]
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d2f3407d9a573d666de4b5bdf10569d73ca9478087346697dcbae6244bfbcd"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "easy-ext"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49457524c7e65648794c98283282a0b7c73b10018e7091f1cdcfff314fd7ae59"
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "eng_fmt"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c263a94ae6bb6421c63a454ad97968f6a6a7dfd3d23aab51441b604d074af3f0"
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.12"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ethnum"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8ff382b2fa527fb7fb06eeebfc5bbb3f17e3cc6b9d70b006c41daa8824adac"
+checksum = "b90ca2580b73ab6a1f724b76ca11ab632df820fd6040c336200d2c1df7b3c82c"
 
 [[package]]
 name = "fast-float"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "futures"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -705,42 +687,46 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.0"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "half"
-version = "1.8.2"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
+dependencies = [
+ "cfg-if",
+ "crunchy",
+]
 
 [[package]]
 name = "hash_hasher"
 version = "2.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
 
@@ -748,59 +734,56 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.1"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dfda62a12f55daeae5015f81b0baea145391cb4520f86c248fc615d72640d12"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
  "rayon",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "home"
-version = "0.5.5"
+version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
+checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.57"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows",
+ "windows-core",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
@@ -816,20 +799,20 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.0.2"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8adf3ddd720272c6ea8bf59463c04e0f93d0bbf7c5439b691bca2987e0270897"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.1",
+ "hashbrown 0.14.5",
  "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -841,33 +824,44 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "is-terminal"
+version = "0.4.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "itoa"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.26"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lexical"
 version = "6.1.1"
@@ -939,23 +933,33 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libm"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
+
+[[package]]
+name = "libredox"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
+dependencies = [
+ "bitflags",
+ "libc",
+]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
@@ -963,27 +967,27 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lz4"
 version = "1.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
 dependencies = [
@@ -999,72 +1003,71 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.6.3"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f232d6ef707e1956a43342693d2a31e72989554d58299d7a88738cc95b0d35c"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.8"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
- "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multiversion"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2c7b9d7fe61760ce5ea19532ead98541f6b4c495d87247aff9826445cf6872a"
+checksum = "c4851161a11d3ad0bf9402d90ffc3967bf231768bfd7aeb61755ad06dbf1a142"
 dependencies = [
  "multiversion-macros",
  "target-features",
 ]
 
 [[package]]
 name = "multiversion-macros"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26a83d8500ed06d68877e9de1dde76c1dbb83885dcdbda4ef44ccbc3fbda2ac8"
+checksum = "79a74ddee9e0c27d2578323c13905793e91622148f138ba29738f9dddb835e90"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "target-features",
 ]
 
@@ -1090,165 +1093,159 @@
 checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "35bd024e8b2ff75562e5f34e7f4905839deb4b22955ef5e73d2fea1b9813cb23"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.4"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba157ca0885411de85d6ca030ba7e2a83a28636056c7c699b07c8b6f7383214"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.43"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.16"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
-name = "num_threads"
-version = "0.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.3.5",
+ "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.27"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "planus"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
@@ -1274,15 +1271,15 @@
 [[package]]
 name = "polars-arrow"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f967c901fa5da4ca7f64e813d1268488ba97e9b3004cefc579ff851c197a1138"
 dependencies = [
  "arrow2",
- "hashbrown 0.14.1",
+ "hashbrown 0.14.5",
  "multiversion",
  "num-traits",
  "polars-error",
  "serde",
  "thiserror",
  "version_check",
 ]
@@ -1291,20 +1288,20 @@
 name = "polars-core"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b24f92fc5b167f668ff85ab9607dfa72e2c09664cacef59297ee8601dee60126"
 dependencies = [
  "ahash",
  "arrow2",
- "bitflags 2.4.0",
+ "bitflags",
  "chrono",
  "comfy-table",
  "either",
- "hashbrown 0.14.1",
- "indexmap 2.0.2",
+ "hashbrown 0.14.5",
+ "indexmap 2.2.6",
  "num-traits",
  "once_cell",
  "polars-arrow",
  "polars-error",
  "polars-row",
  "polars-utils",
  "rand",
@@ -1364,15 +1361,15 @@
 [[package]]
 name = "polars-lazy"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c33762ec2a55e01c9f8776b34db86257c70a0a3b3929bd4eb91a52aacf61456"
 dependencies = [
  "ahash",
- "bitflags 2.4.0",
+ "bitflags",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-pipe",
@@ -1389,15 +1386,15 @@
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e825575c96302d2daedfc205a0062180033c92c55bcd6aafc4e109d4d8849ed0"
 dependencies = [
  "argminmax",
  "arrow2",
  "either",
- "indexmap 2.0.2",
+ "indexmap 2.2.6",
  "memchr",
  "polars-arrow",
  "polars-core",
  "polars-utils",
  "serde",
  "smartstring",
  "version_check",
@@ -1406,15 +1403,15 @@
 [[package]]
 name = "polars-pipe"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f2bc9a12da9ed043fb0cb51dbcb87b365e4845b7ab6399d7a81e838460c6974"
 dependencies = [
  "enum_dispatch",
- "hashbrown 0.14.1",
+ "hashbrown 0.14.5",
  "num-traits",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-plan",
  "polars-row",
@@ -1439,15 +1436,15 @@
  "polars-ops",
  "polars-time",
  "polars-utils",
  "rayon",
  "regex",
  "serde",
  "smartstring",
- "strum_macros 0.25.2",
+ "strum_macros 0.25.3",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1496,25 +1493,31 @@
 [[package]]
 name = "polars-utils"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c326708a370d71dc6e11a8f4bbc10a8479e1c314dc048ba73543b815cd0bf339"
 dependencies = [
  "ahash",
- "hashbrown 0.14.1",
+ "hashbrown 0.14.5",
  "num-traits",
  "once_cell",
  "polars-error",
  "rayon",
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
+name = "powerfmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro-error"
@@ -1538,17 +1541,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.67"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d433d9f1a3e8c1263d9456598b16fec66f4acc9a74dacffd35c7bb09b3a1328"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "project-root"
 version = "0.2.2"
@@ -1591,17 +1594,17 @@
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.3"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f47b0777feb17f61eea78667d61103758b243a871edc09a7786500a50467b605"
+checksum = "4c10808ee7250403bedb24bc30c32493e93875fef7ba3e4292226fe924f398bd"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
@@ -1641,17 +1644,17 @@
  "polars-plan",
  "pyo3",
  "thiserror",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1692,164 +1695,155 @@
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.8.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c27db03db7734835b3f53954b534c91069375ce6ccaa2e065441e07d9b6cdb1"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.12.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ce3fb6ad83f861aac485e76e1985cd109d9a3713802152be56c3b1f0e0658ed"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "readonly"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8f439da1766942fe069954da6058b2e6c1760eb878bae76f5be9fc29f56f574"
+checksum = "a25d631e41bfb5fdcde1d4e2215f62f7f0afa3ff11e26563765bd6ea1d229aeb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
-dependencies = [
- "bitflags 1.3.2",
-]
-
-[[package]]
-name = "redox_syscall"
-version = "0.3.5"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.3"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
- "redox_syscall 0.2.16",
+ "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.9.5"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "697061221ea1b4a94a624f67d0ae2bfe4e22b8a17b6a192afb11046542cc8c47"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
- "regex-syntax 0.7.5",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.8"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2f401f4955220693b56f8ec66ee9c78abffd8d1c4f23dc41a23839eb88f0795"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.7.5",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.5"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb5fb1acd8a1a18b3dd5be62d25485eb770e05afb408a9627d14d451bae12da"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.0",
+ "bitflags",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "955d28af4278de8121b7ebeb796b6a45735dc01436d898801014aced2773a3d6"
 
 [[package]]
 name = "ryu"
-version = "1.0.15"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.19"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad977052201c6de01a8ef2aa3378c4bd23217a056337d1d6da40468d267a4fb0"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-this-or-that"
 version = "0.4.2"
@@ -1857,28 +1851,28 @@
 checksum = "634c5a3cb041e56cc2964386151c67d520f845445789da3bd46bfb1c94f5e3bb"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.107"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b420ce6e3d8bd882e9b243c6eed35dbc9a6110c9769e74b584e0d68d1f20c65"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1890,44 +1884,14 @@
  "indexmap 1.9.3",
  "ryu",
  "serde",
  "yaml-rust",
 ]
 
 [[package]]
-name = "signal-hook"
-version = "0.3.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8621587d4798caf8eb44879d42e56b9a93ea5dcd315a6487c357130095b62801"
-dependencies = [
- "libc",
- "signal-hook-registry",
-]
-
-[[package]]
-name = "signal-hook-mio"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "29ad2e15f37ec9a6cc544097b78a1ec90001e9f71b81338ca39f430adaca99af"
-dependencies = [
- "libc",
- "mio",
- "signal-hook",
-]
-
-[[package]]
-name = "signal-hook-registry"
-version = "1.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "slab"
@@ -1966,30 +1930,30 @@
  "serde_json",
  "slog",
  "time",
 ]
 
 [[package]]
 name = "slog-term"
-version = "2.9.0"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87d29185c55b7b258b4f120eab00f48557d4d9bc814f41713f449d35b0f8977c"
+checksum = "b6e022d0b998abfe5c3782c1f03551a596269450ccd677ea51c56f8b214610e8"
 dependencies = [
- "atty",
+ "is-terminal",
  "slog",
  "term",
  "thread_local",
  "time",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
@@ -1997,20 +1961,20 @@
  "serde",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.4"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4031e820eb552adee9295814c0ced9e5cf38ddf1e8b7d566d6de8e2538ea989e"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "sqlparser"
 version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2eaa1e88e78d2c2460d78b7dc3f0c08dbb606ab4222f9aff36f420d36e307d87"
@@ -2028,42 +1992,42 @@
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
 name = "strum"
-version = "0.24.1"
+version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "063e6045c0e62079840579a7e47a355ae92f60eb74daaf156fb1e84ba164e63f"
+checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
 
 [[package]]
 name = "strum_macros"
-version = "0.24.3"
+version = "0.25.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
+checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 1.0.109",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "strum_macros"
-version = "0.25.2"
+version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad8d03b598d3d0fff69bf533ee3ef19b8eeb342729596df84bcc7e1f96ec4059"
+checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -2071,28 +2035,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.37"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7303ef2c05cd654186cb250d29049a24840ca25d2747c25c0381c8d9e2f582e8"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.29.10"
+version = "0.29.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a18d114d420ada3a891e6bc8e96a2023402203296a47cdd65083377dad18ba5"
+checksum = "cd727fc423c2060f6c92d9534cef765c65a6ed3f428a03d7def74a8c4348e666"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "winapi",
@@ -2102,23 +2066,23 @@
 name = "take_mut"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "target-features"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb5fa503293557c5158bd215fdc225695e567a77e453f5d4452a50a193969bd"
+checksum = "c1bbb9f3c5c463a01705937a24fdabc5047929ac764b2d5b9cf681c1f5041ed5"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.11"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
@@ -2137,77 +2101,78 @@
  "dirs-next",
  "rustversion",
  "winapi",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.49"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1177e8c6d7ede7afde3585fd2513e611227efd6481bd78d2e82ba1ce16557ed4"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.49"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10712f02019e9288794769fba95cd6847df9874d49d871d062172f9dd41bc4cc"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.29"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "426f806f4089c493dcac0d24c29c01e2c38baf8e30f1b716ee37e83d200b18fe"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
- "libc",
- "num_threads",
+ "num-conv",
+ "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.15"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ad70d68dba9e1f8aceda7aa6711965dfec1cac869f311a51bd08b3a2ccbce20"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
+ "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.32.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17ed6077ed6cd6c74735e21f37eb16dc3935f96878b1fe961074089cc80893f9"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "libc",
  "mio",
  "pin-project-lite",
  "socket2",
  "windows-sys 0.48.0",
@@ -2223,17 +2188,17 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -2258,65 +2223,65 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.63",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -2333,20 +2298,20 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows"
-version = "0.48.0"
+name = "windows-core"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -2482,28 +2447,48 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xxhash-rust"
-version = "0.8.7"
+version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9828b178da53440fa9c766a3d2f73f7cf5d0ac1fe3980c1e5018d899fd19e07b"
+checksum = "927da81e25be1e1a2901d59b81b37dd2efd1fc9c9345a55007f09bf5a2d3ee03"
 
 [[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
+name = "zerocopy"
+version = "0.7.34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
+dependencies = [
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.7.34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.63",
+]
+
+[[package]]
 name = "zstd"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
  "zstd-safe",
 ]
@@ -2516,15 +2501,14 @@
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.8+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
- "libc",
  "pkg-config",
 ]
```

### Comparing `altrios-0.2.2/rust/Cargo.toml` & `altrios-0.2.3/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/pyproject.toml` & `altrios-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0"]
 build-backend = "maturin"
 
 [project]
 name = "altrios"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name = "ALTRIOS Team", email = "altrios@nrel.gov" },
     { name = "Chad Baker, Lead Developer" },
     { name = "Nick Reinicke, Developer" },
     { name = "Matt Bruchon, Developer" },
     { name = "Saad Akhtar, Developer" },
     { name = "Steven Shi, Developer" },
```

### Comparing `altrios-0.2.2/python/altrios/stringline_old.py` & `altrios-0.2.3/python/altrios/stringline_old.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/speed_limit_train_sim_demo.py` & `altrios-0.2.3/python/altrios/demos/speed_limit_train_sim_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
     network,
     alt.SpeedLimitTrainSimVec([train_sim]),
     [est_time_net],
     False,
     False,
 )[0]
 
+# uncomment this line to see example of logging functionality
+# alt.utils.set_log_level("DEBUG")
+
 t0 = time.perf_counter()
 train_sim.walk_timed_path(
     network=network,
     timed_path=timed_link_path,
 )
 t1 = time.perf_counter()
 print(f'Time to simulate: {t1 - t0:.5g}')
```

### Comparing `altrios-0.2.2/python/altrios/demos/speed_limit_simple_corr_demo.py` & `altrios-0.2.3/python/altrios/demos/speed_limit_simple_corr_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/sim_manager_demo.py` & `altrios-0.2.3/python/altrios/demos/sim_manager_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/version_migration_demo.py` & `altrios-0.2.3/python/altrios/demos/version_migration_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/set_speed_simple_corr_demo.py` & `altrios-0.2.3/python/altrios/demos/set_speed_simple_corr_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/rollout_demo.py` & `altrios-0.2.3/python/altrios/demos/rollout_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/set_speed_train_sim_demo.py` & `altrios-0.2.3/python/altrios/demos/set_speed_train_sim_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/test_demos.py` & `altrios-0.2.3/python/altrios/demos/test_demos.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/conv_demo.py` & `altrios-0.2.3/python/altrios/demos/conv_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/demos/bel_demo.py` & `altrios-0.2.3/python/altrios/demos/bel_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/train_planner.py` & `altrios-0.2.3/python/altrios/train_planner.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/output_12072022.csv` & `altrios-0.2.3/python/altrios/output_12072022.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/utilities.py` & `altrios-0.2.3/python/altrios/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module for general functions, classes, and unit conversion factors."""
 
+from __future__ import annotations
 import re
 import numpy as np
 from typing import Tuple, Union, Optional, Dict, Any, TYPE_CHECKING
 import pandas as pd
 import datetime
 import numpy.typing as npt
 import logging
@@ -260,23 +261,71 @@
     )
     return new_signal
 
 
 def print_dt():
     print(datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
 
+def set_log_level(level: str | int) -> int:
+    """
+    Sets logging level for both Python and Rust.
+    The default logging level is WARNING (30).
+    https://docs.python.org/3/library/logging.html#logging-levels
 
-def set_log_level(level: Union[str, int]):
+    Parameters
+    ----------
+    level: `str` | `int`
+        Logging level to set. `str` level name or `int` logging level
+        
+        =========== ================
+        Level       Numeric value
+        =========== ================
+        CRITICAL    50
+        ERROR       40
+        WARNING     30
+        INFO        20
+        DEBUG       10
+        NOTSET      0
+    
+    Returns
+    -------
+    `int`
+        Previous log level
+    """
     # Map string name to logging level
-    if isinstance(level, str):
-        level = logging._nameToLevel[level]
-    # Set logging level
-    logging.getLogger("").setLevel(level)
 
+    allowed_args = [
+        ("CRITICAL", 50),
+        ("ERROR", 40),
+        ("WARNING", 30),
+        ("INFO", 20),
+        ("DEBUG", 10),
+        ("NOTSET", 0),
+        # no logging of anything ever!
+        ("NONE", logging.CRITICAL + 1),
+    ]
+    allowed_str_args = [a[0] for a in allowed_args]
+    allowed_int_args = [a[1] for a in allowed_args]
+
+    err_str = f"Invalid arg: '{level}'.  See doc string:\n{set_log_level.__doc__}"
 
+    if isinstance(level, str):
+        assert level.upper() in allowed_str_args, err_str
+        level = logging._nameToLevel[level.upper()]
+    else:
+        assert level in allowed_int_args, err_str
+
+    # Extract previous log level and set new log level
+    python_logger  = logging.getLogger("altrios")
+    previous_level = python_logger .level
+    python_logger .setLevel(level)
+    rust_logger = logging.getLogger("altrios_core")
+    rust_logger.setLevel(level)
+    return previous_level
+    
 def disable_logging():
     set_log_level(logging.CRITICAL + 1)
 
 
 def enable_logging():
     set_log_level(logging.WARNING)
 
@@ -316,8 +365,8 @@
         
     print(f"Saved {dest_file.name} to {dest_file}")
 
 def show_plots() -> bool:
     """
     Returns true if plots should be displayed
     """
-    return os.environ.get("SHOW_PLOTS", "true").lower() == "true"        
+    return os.environ.get("SHOW_PLOTS", "true").lower() == "true"
```

### Comparing `altrios-0.2.2/python/altrios/stringline.py` & `altrios-0.2.3/python/altrios/stringline.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/__init__.py` & `altrios-0.2.3/python/altrios/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 from altrios.utilities import set_param_from_path  # noqa: F401
 from altrios.utilities import copy_demo_files  # noqa: F401
 from altrios import utilities as utils
 from altrios.utilities import package_root, resources_root
 # make everything in altrios_pyo3 available here
 from altrios.altrios_pyo3 import *
 
+DEFAULT_LOGGING_CONFIG = dict(
+    format="%(asctime)s.%(msecs)03d | %(filename)s:%(lineno)s | %(levelname)s: %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
+)
 
 # Set up logging
-logging.basicConfig(
-    format="%(asctime)s.%(msecs)03d | %(filename)s#%(lineno)s | %(levelname)s: %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S"
-)
-utils.enable_logging()
+logging.basicConfig(**DEFAULT_LOGGING_CONFIG)
+logger = logging.getLogger(__name__)
 
 def __array__(self):
     return np.array(self.tolist())
 
 
 setattr(ReversibleEnergyStorage, "from_excel", classmethod(_res_from_excel))  # noqa: F405
 setattr(Pyo3VecWrapper, "__array__", __array__)  # noqa: F405
```

### Comparing `altrios-0.2.2/python/altrios/metric_calculator.py` & `altrios-0.2.3/python/altrios/metric_calculator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv` & `altrios-0.2.3/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv` & `altrios-0.2.3/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv` & `altrios-0.2.3/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv` & `altrios-0.2.3/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv` & `altrios-0.2.3/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv` & `altrios-0.2.3/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/Default Demand StoBar.csv` & `altrios-0.2.3/python/altrios/resources/Default Demand StoBar.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/rolling_stock/rail_vehicles.csv` & `altrios-0.2.3/python/altrios/resources/rolling_stock/rail_vehicles.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/trains/train_res_temp.yaml` & `altrios-0.2.3/python/altrios/resources/trains/train_res_temp.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx` & `altrios-0.2.3/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml` & `altrios-0.2.3/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml` & `altrios-0.2.3/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/demo_data/speed_trace.csv` & `altrios-0.2.3/python/altrios/resources/demo_data/speed_trace.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/TimedPaths.csv` & `altrios-0.2.3/python/altrios/resources/TimedPaths.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/networks/Taconite-NoBalloon.yaml` & `altrios-0.2.3/python/altrios/resources/networks/Taconite-NoBalloon.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/networks/links_test.yaml` & `altrios-0.2.3/python/altrios/resources/networks/links_test.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/networks/Taconite_v0.1.6.yaml` & `altrios-0.2.3/python/altrios/resources/networks/Taconite_v0.1.6.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv` & `altrios-0.2.3/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/networks/simple_corridor_network.yaml` & `altrios-0.2.3/python/altrios/resources/networks/simple_corridor_network.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/resources/networks/Taconite.yaml` & `altrios-0.2.3/python/altrios/resources/networks/Taconite.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/defaults.py` & `altrios-0.2.3/python/altrios/defaults.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/rollout.py` & `altrios-0.2.3/python/altrios/rollout.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/loaders/powertrain_components.py` & `altrios-0.2.3/python/altrios/loaders/powertrain_components.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/sim_manager.py` & `altrios-0.2.3/python/altrios/sim_manager.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_consist.py` & `altrios-0.2.3/python/altrios/tests/test_consist.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_rail_vehicles.py` & `altrios-0.2.3/python/altrios/tests/test_rail_vehicles.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_powertrain_fuel_conv.py` & `altrios-0.2.3/python/altrios/tests/test_powertrain_fuel_conv.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_utilities.py` & `altrios-0.2.3/python/altrios/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_powertrain_generator.py` & `altrios-0.2.3/python/altrios/tests/test_powertrain_generator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_locomotive.py` & `altrios-0.2.3/python/altrios/tests/test_locomotive.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_powertrain_edrive.py` & `altrios-0.2.3/python/altrios/tests/test_powertrain_edrive.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_consist_sim.py` & `altrios-0.2.3/python/altrios/tests/test_consist_sim.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_multi_obj_cal_and_val.py` & `altrios-0.2.3/python/altrios/tests/test_multi_obj_cal_and_val.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_powertrain_res.py` & `altrios-0.2.3/python/altrios/tests/test_powertrain_res.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_metric_calculator.py` & `altrios-0.2.3/python/altrios/tests/test_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/mock_resources.py` & `altrios-0.2.3/python/altrios/tests/mock_resources.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/tests/test_locomotive_simulation.py` & `altrios-0.2.3/python/altrios/tests/test_locomotive_simulation.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/altrios_pyo3.pyi` & `altrios-0.2.3/python/altrios/altrios_pyo3.pyi`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/python/altrios/optimization/cal_and_val.py` & `altrios-0.2.3/python/altrios/optimization/cal_and_val.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/README.md` & `altrios-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ### Python Setup
 
 1. Python installation options:
    - Option 1 -- Python: https://www.python.org/downloads/. We recommend Python 3.10. Be sure to check the `Add to PATH` option during installation.
    - Option 2 -- Anaconda: we recommend https://docs.conda.io/en/latest/miniconda.html.
 1. Setup a python environment. ALTRIOS can work with Python 3.9, or 3.10, but we recommend 3.10 for better performance and user experience. Create a python environment for ALTRIOS with either of two methods:
    - Option 1 -- [Python Venv](https://docs.python.org/3/library/venv.html)
-     1. Navigate to the ALTRIOS folder you just cloned or any folder you'd like for using ALTRIOS. Remember the folder you use!
+     1. Navigate to your project folder in which you'd like to store model data and run ALTRIOS.
      1. Assuming you have Python 3.10 installed, run `python3.10 -m venv altrios-venv` in your terminal enviroment (we recommend PowerShell in Windows, which comes pre-installed). This tells Python 3.10 to use the `venv` module to create a virtual environment (which will be ignored by git if named `altrios-venv`) in the `ALTRIOS/altrios-venv/`.
      1. Activate the environment you just created to install packages or anytime you're running ALTRIOS:
         - Mac and Linux: `source altrios-venv/bin/activate`
         - Windows: `altrios-venv/Scripts/activate.bat` in a windows command prompt or power shell or `source ./altrios-venv/scripts/activate` in git bash terminal
         - When the environment is activated, your terminal session will have a decorator that looks like `(altrios-venv)`.
    - Option 2 -- Anaconda:
      1. Open an Anaconda prompt (in Windows, we recommend Anaconda Powershell Prompt) and run the command `conda create -n altrios python=3.10` to create an Anaconda environment named `altrios`.
```

### Comparing `altrios-0.2.2/LICENSE.md` & `altrios-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.2/PKG-INFO` & `altrios-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: altrios
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: pandas >=2
 Requires-Dist: numpy
@@ -55,15 +55,15 @@
 ### Python Setup
 
 1. Python installation options:
    - Option 1 -- Python: https://www.python.org/downloads/. We recommend Python 3.10. Be sure to check the `Add to PATH` option during installation.
    - Option 2 -- Anaconda: we recommend https://docs.conda.io/en/latest/miniconda.html.
 1. Setup a python environment. ALTRIOS can work with Python 3.9, or 3.10, but we recommend 3.10 for better performance and user experience. Create a python environment for ALTRIOS with either of two methods:
    - Option 1 -- [Python Venv](https://docs.python.org/3/library/venv.html)
-     1. Navigate to the ALTRIOS folder you just cloned or any folder you'd like for using ALTRIOS. Remember the folder you use!
+     1. Navigate to your project folder in which you'd like to store model data and run ALTRIOS.
      1. Assuming you have Python 3.10 installed, run `python3.10 -m venv altrios-venv` in your terminal enviroment (we recommend PowerShell in Windows, which comes pre-installed). This tells Python 3.10 to use the `venv` module to create a virtual environment (which will be ignored by git if named `altrios-venv`) in the `ALTRIOS/altrios-venv/`.
      1. Activate the environment you just created to install packages or anytime you're running ALTRIOS:
         - Mac and Linux: `source altrios-venv/bin/activate`
         - Windows: `altrios-venv/Scripts/activate.bat` in a windows command prompt or power shell or `source ./altrios-venv/scripts/activate` in git bash terminal
         - When the environment is activated, your terminal session will have a decorator that looks like `(altrios-venv)`.
    - Option 2 -- Anaconda:
      1. Open an Anaconda prompt (in Windows, we recommend Anaconda Powershell Prompt) and run the command `conda create -n altrios python=3.10` to create an Anaconda environment named `altrios`.
```

