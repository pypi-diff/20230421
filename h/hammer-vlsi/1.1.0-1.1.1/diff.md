# Comparing `tmp/hammer_vlsi-1.1.0.tar.gz` & `tmp/hammer_vlsi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hammer_vlsi-1.1.0.tar", max compression
+gzip compressed data, was "hammer_vlsi-1.1.1.tar", max compression
```

## Comparing `hammer_vlsi-1.1.0.tar` & `hammer_vlsi-1.1.1.tar`

### file list

```diff
@@ -1,402 +1,402 @@
--rw-r--r--   0        0        0     1568 2023-03-20 22:33:21.782222 hammer_vlsi-1.1.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-03-20 22:33:21.782222 hammer_vlsi-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/__init__.py
--rw-r--r--   0        0        0    20617 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/cadence/__init__.py
--rw-r--r--   0        0        0      436 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/cadence/defaults.yml
--rw-r--r--   0        0        0      456 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/cadence/defaults_types.yml
--rw-r--r--   0        0        0        0 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/mentor/__init__.py
--rw-r--r--   0        0        0      571 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/mentor/defaults.yml
--rw-r--r--   0        0        0      600 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/mentor/defaults_types.yml
--rw-r--r--   0        0        0        0 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/openroad/__init__.py
--rw-r--r--   0        0        0      189 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/openroad/defaults.yml
--rw-r--r--   0        0        0      207 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/openroad/defaults_types.yml
--rw-r--r--   0        0        0     3592 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/synopsys/__init__.py
--rw-r--r--   0        0        0      494 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/synopsys/defaults.yml
--rw-r--r--   0        0        0      415 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/synopsys/defaults_types.yml
--rw-r--r--   0        0        0     3653 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/common/vivado/vivado_core.py
--rw-r--r--   0        0        0      147 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/config/__init__.py
--rw-r--r--   0        0        0      434 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/config/builtins.yml
--rw-r--r--   0        0        0       81 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/config/common.py
--rw-r--r--   0        0        0    51427 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/config/config_src.py
--rw-r--r--   0        0        0    46353 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/config/defaults.yml
--rw-r--r--   0        0        0    18306 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/config/defaults_types.yml
--rw-r--r--   0        0        0     3904 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/config/yaml2json.py
--rw-r--r--   0        0        0     1467 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/icv/README.md
--rw-r--r--   0        0        0     7027 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/icv/__init__.py
--rw-r--r--   0        0        0     1305 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/icv/defaults.yml
--rw-r--r--   0        0        0     6551 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/magic/__init__.py
--rw-r--r--   0        0        0      617 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/magic/defaults.yml
--rw-r--r--   0        0        0      516 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/mockdrc/__init__.py
--rw-r--r--   0        0        0      421 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/nop/__init__.py
--rw-r--r--   0        0        0     4221 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/openroad/__init__.py
--rw-r--r--   0        0        0      380 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/drc/openroad/defaults.yml
--rw-r--r--   0        0        0    11337 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/formal/conformal/__init__.py
--rw-r--r--   0        0        0      963 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/formal/conformal/defaults.yml
--rwxr-xr-x   0        0        0    16492 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/generate_properties.py
--rw-r--r--   0        0        0      251 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/logging/__init__.py
--rw-r--r--   0        0        0     8650 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/logging/logging.py
--rw-r--r--   0        0        0     2033 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/logging/test.py
--rw-r--r--   0        0        0     9010 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/lvs/icv/__init__.py
--rw-r--r--   0        0        0     1454 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/lvs/icv/defaults.yml
--rw-r--r--   0        0        0      600 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/lvs/mocklvs/__init__.py
--rw-r--r--   0        0        0     8263 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/lvs/netgen/__init__.py
--rw-r--r--   0        0        0      628 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/lvs/netgen/defaults.yml
--rw-r--r--   0        0        0      480 2023-03-20 22:33:21.794222 hammer_vlsi-1.1.0/hammer/lvs/nop/__init__.py
--rw-r--r--   0        0        0    56234 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/innovus/__init__.py
--rw-r--r--   0        0        0     1681 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/innovus/defaults.yml
--rw-r--r--   0        0        0     2510 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/innovus/dump_stackup_to_json.tcl
--rw-r--r--   0        0        0     3461 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/mockpar/__init__.py
--rw-r--r--   0        0        0       77 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/mockpar/defaults.yml
--rw-r--r--   0        0        0      966 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/nop/__init__.py
--rw-r--r--   0        0        0     4816 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/openroad/README.md
--rw-r--r--   0        0        0    85243 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/openroad/__init__.py
--rw-r--r--   0        0        0     4727 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/openroad/defaults.yml
--rw-r--r--   0        0        0     1155 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/openroad/defaults_types.yml
--rw-r--r--   0        0        0     1926 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/par/vivado/__init__.py
--rw-r--r--   0        0        0    13460 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/pcb/generic/__init__.py
--rw-r--r--   0        0        0      605 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/pcb/generic/defaults.yml
--rw-r--r--   0        0        0     9710 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/power/joules/__init__.py
--rw-r--r--   0        0        0      450 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/power/joules/defaults.yml
--rw-r--r--   0        0        0    41055 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/power/voltus/__init__.py
--rw-r--r--   0        0        0     1187 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/power/voltus/defaults.yml
--rw-r--r--   0        0        0        0 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/py.typed
--rw-r--r--   0        0        0     1723 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/shell/get_config.py
--rw-r--r--   0        0        0     3538 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/shell/hammer_generate_mdf.py
--rw-r--r--   0        0        0      147 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/shell/hammer_shell_test.py
--rw-r--r--   0        0        0      188 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/shell/hammer_vlsi.py
--rw-r--r--   0        0        0      691 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/shell/readlink_array.py
--rw-r--r--   0        0        0     1532 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/shell/yaml2json.py
--rw-r--r--   0        0        0     1324 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sim/mocksim/__init__.py
--rw-r--r--   0        0        0       76 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sim/mocksim/defaults.yml
--rw-r--r--   0        0        0    17431 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sim/vcs/__init__.py
--rw-r--r--   0        0        0      699 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sim/vcs/defaults.yml
--rw-r--r--   0        0        0    19752 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sim/xcelium/__init__.py
--rw-r--r--   0        0        0     1332 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sim/xcelium/defaults.yml
--rw-r--r--   0        0        0      804 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sim/xcelium/defaults_types.yml
--rw-r--r--   0        0        0      701 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sram_generator/mocksram_generator/__init__.py
--rw-r--r--   0        0        0      470 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/sram_generator/nop/__init__.py
--rw-r--r--   0        0        0    18000 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/genus/__init__.py
--rw-r--r--   0        0        0      524 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/genus/defaults.yml
--rw-r--r--   0        0        0     2352 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/mocksynth/__init__.py
--rw-r--r--   0        0        0      211 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/mocksynth/defaults.yml
--rw-r--r--   0        0        0      354 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/nop/__init__.py
--rw-r--r--   0        0        0     2467 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/__init__.py
--rw-r--r--   0        0        0      899 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/defaults.yml
--rw-r--r--   0        0        0      144 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/board.tcl
--rw-r--r--   0        0        0     1419 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/init.tcl
--rw-r--r--   0        0        0      749 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/ip.tcl
--rw-r--r--   0        0        0      360 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/mcs.tcl
--rw-r--r--   0        0        0      247 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/msg.tcl
--rw-r--r--   0        0        0     1847 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/par.tcl
--rw-r--r--   0        0        0      342 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/paths.tcl
--rw-r--r--   0        0        0      426 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/project.tcl
--rw-r--r--   0        0        0     1291 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/prologue.tcl
--rwxr-xr-x   0        0        0      226 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/run-par
--rwxr-xr-x   0        0        0      189 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/run-synthesis
--rw-r--r--   0        0        0      291 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/syn.tcl
--rw-r--r--   0        0        0       26 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/vc707.xdc
--rw-r--r--   0        0        0      183 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/vivado_setup.sh
--rw-r--r--   0        0        0    14891 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/yosys/__init__.py
--rw-r--r--   0        0        0      630 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/yosys/defaults.yml
--rw-r--r--   0        0        0      594 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/synthesis/yosys/defaults_types.yml
--rw-r--r--   0        0        0    59569 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/tech/__init__.py
--rw-r--r--   0        0        0      921 2023-03-20 22:33:21.798222 hammer_vlsi-1.1.0/hammer/tech/specialcells.py
--rw-r--r--   0        0        0    18266 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/tech/stackup.py
--rw-r--r--   0        0        0     4117 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/README.md
--rw-r--r--   0        0        0    13924 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/__init__.py
--rw-r--r--   0        0        0    47808 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/asap7.tech.json
--rw-r--r--   0        0        0     1450 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/calibre.layerprops
--rw-r--r--   0        0        0     3488 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/defaults.yml
--rw-r--r--   0        0        0      155 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/defaults_types.yml
--rwxr-xr-x   0        0        0     4305 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/gds_scale.py
--rw-r--r--   0        0        0      314 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/latch_map.v
--rw-r--r--   0        0        0      657 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/lefdefLayer.map
--rwxr-xr-x   0        0        0     3622 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram-cache-gen.py
--rw-r--r--   0        0        0    54410 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram-cache.json
--rw-r--r--   0        0        0     7899 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/__init__.py
--rw-r--r--   0        0        0    10084 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds
--rw-r--r--   0        0        0    10784 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds
--rw-r--r--   0        0        0    17108 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds
--rw-r--r--   0        0        0    19564 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds
--rw-r--r--   0        0        0    19916 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds
--rw-r--r--   0        0        0    22376 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds
--rw-r--r--   0        0        0    31156 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds
--rw-r--r--   0        0        0     6580 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds
--rw-r--r--   0        0        0     7806 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds
--rw-r--r--   0        0        0     8510 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds
--rw-r--r--   0        0        0    12022 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds
--rw-r--r--   0        0        0    20098 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds
--rw-r--r--   0        0        0    22558 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds
--rw-r--r--   0        0        0    23610 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds
--rw-r--r--   0        0        0    30634 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds
--rw-r--r--   0        0        0     6054 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds
--rw-r--r--   0        0        0     6756 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds
--rw-r--r--   0        0        0    58904 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds
--rw-r--r--   0        0        0    16760 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds
--rw-r--r--   0        0        0    23080 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds
--rw-r--r--   0        0        0    23784 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds
--rw-r--r--   0        0        0    30808 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds
--rw-r--r--   0        0        0     6228 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds
--rw-r--r--   0        0        0    23962 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds
--rw-r--r--   0        0        0    10784 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds
--rw-r--r--   0        0        0     7280 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds
--rw-r--r--   0        0        0    59078 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds
--rw-r--r--   0        0        0    16934 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds
--rw-r--r--   0        0        0    30982 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds
--rw-r--r--   0        0        0     6402 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds
--rw-r--r--   0        0        0    58556 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds
--rw-r--r--   0        0        0    11140 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds
--rw-r--r--   0        0        0    11492 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds
--rw-r--r--   0        0        0    11844 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds
--rw-r--r--   0        0        0    16408 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds
--rw-r--r--   0        0        0    17112 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds
--rw-r--r--   0        0        0     5880 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds
--rw-r--r--   0        0        0    18918 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds
--rw-r--r--   0        0        0    32966 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds
--rw-r--r--   0        0        0     8378 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds
--rw-r--r--   0        0        0    11890 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds
--rw-r--r--   0        0        0    17858 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds
--rw-r--r--   0        0        0    31906 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds
--rw-r--r--   0        0        0     7322 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds
--rw-r--r--   0        0        0    10834 2023-03-20 22:33:21.802222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds
--rw-r--r--   0        0        0    18210 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds
--rw-r--r--   0        0        0    23478 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds
--rw-r--r--   0        0        0    32258 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds
--rw-r--r--   0        0        0    32962 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds
--rw-r--r--   0        0        0    38230 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds
--rw-r--r--   0        0        0     7674 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds
--rw-r--r--   0        0        0    11186 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds
--rw-r--r--   0        0        0    18562 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds
--rw-r--r--   0        0        0    25586 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds
--rw-r--r--   0        0        0    32610 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds
--rw-r--r--   0        0        0     8026 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds
--rw-r--r--   0        0        0    11538 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds
--rw-r--r--   0        0        0     7051 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef
--rw-r--r--   0        0        0     7398 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef
--rw-r--r--   0        0        0    11742 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef
--rw-r--r--   0        0        0    13264 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef
--rw-r--r--   0        0        0    13537 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef
--rw-r--r--   0        0        0    15249 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef
--rw-r--r--   0        0        0    21091 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef
--rw-r--r--   0        0        0     4754 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef
--rw-r--r--   0        0        0     5494 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef
--rw-r--r--   0        0        0     6031 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef
--rw-r--r--   0        0        0     8355 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef
--rw-r--r--   0        0        0    13650 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef
--rw-r--r--   0        0        0    15362 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef
--rw-r--r--   0        0        0    15985 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef
--rw-r--r--   0        0        0    20654 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef
--rw-r--r--   0        0        0     4352 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef
--rw-r--r--   0        0        0     4888 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef
--rw-r--r--   0        0        0    39648 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef
--rw-r--r--   0        0        0    11450 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef
--rw-r--r--   0        0        0    15574 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef
--rw-r--r--   0        0        0    16119 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef
--rw-r--r--   0        0        0    20788 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef
--rw-r--r--   0        0        0     4484 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef
--rw-r--r--   0        0        0    16251 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef
--rw-r--r--   0        0        0     7417 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef
--rw-r--r--   0        0        0     5107 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef
--rw-r--r--   0        0        0    39781 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef
--rw-r--r--   0        0        0    11583 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef
--rw-r--r--   0        0        0    20958 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef
--rw-r--r--   0        0        0     4611 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef
--rw-r--r--   0        0        0    39308 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef
--rw-r--r--   0        0        0     7675 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef
--rw-r--r--   0        0        0     7946 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef
--rw-r--r--   0        0        0     8218 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef
--rw-r--r--   0        0        0    11176 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef
--rw-r--r--   0        0        0    11716 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef
--rw-r--r--   0        0        0     4218 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef
--rw-r--r--   0        0        0    12982 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef
--rw-r--r--   0        0        0    22452 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef
--rw-r--r--   0        0        0     5940 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef
--rw-r--r--   0        0        0     8262 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef
--rw-r--r--   0        0        0    12165 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef
--rw-r--r--   0        0        0    21631 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef
--rw-r--r--   0        0        0     5123 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef
--rw-r--r--   0        0        0     7446 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef
--rw-r--r--   0        0        0    12437 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef
--rw-r--r--   0        0        0    15987 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef
--rw-r--r--   0        0        0    21899 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef
--rw-r--r--   0        0        0    22455 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef
--rw-r--r--   0        0        0    26004 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef
--rw-r--r--   0        0        0     5403 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef
--rw-r--r--   0        0        0     7718 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef
--rw-r--r--   0        0        0    12708 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef
--rw-r--r--   0        0        0    17441 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef
--rw-r--r--   0        0        0    22174 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef
--rw-r--r--   0        0        0     5670 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef
--rw-r--r--   0        0        0     7988 2023-03-20 22:33:21.806223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef
--rw-r--r--   0        0        0    15410 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15401 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15267 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15364 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15186 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15435 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15305 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15394 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15242 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15198 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15046 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15345 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15211 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15504 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15294 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15495 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15285 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15372 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15363 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15267 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15363 2023-03-20 22:33:21.810222 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15267 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15354 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15258 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15386 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15224 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15368 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15206 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28859 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28513 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28859 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28513 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28846 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28500 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28846 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28500 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28793 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28447 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28793 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28447 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28602 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28256 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28780 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28434 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28792 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28534 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28792 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28534 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28869 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28555 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28869 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28555 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28869 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28555 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28856 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28542 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28856 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28542 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0      773 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/asap7/srams.txt
--rw-r--r--   0        0        0      576 2023-03-20 22:33:21.814223 hammer_vlsi-1.1.0/hammer/technology/nangate45/README.md
--rw-r--r--   0        0        0      365 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nangate45/__init__.py
--rw-r--r--   0        0        0      952 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nangate45/defaults.yml
--rw-r--r--   0        0        0     5912 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nangate45/nangate45.tech.json
--rw-r--r--   0        0        0     1554 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nangate45/sram-cache.json
--rw-r--r--   0        0        0     2835 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nangate45/sram_compiler/__init__.py
--rw-r--r--   0        0        0      116 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nop/__init__.py
--rw-r--r--   0        0        0       33 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nop/defaults.yml
--rw-r--r--   0        0        0       82 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/nop/nop.tech.json
--rw-r--r--   0        0        0     6649 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/README.md
--rw-r--r--   0        0        0    14127 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/__init__.py
--rw-r--r--   0        0        0     5035 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/defaults.yml
--rw-r--r--   0        0        0      711 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/defaults_types.yml
--rw-r--r--   0        0        0      899 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/cells-gen.py
--rw-r--r--   0        0        0    11554 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/cells.txt
--rw-r--r--   0        0        0     2907 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/fill.json
--rwxr-xr-x   0        0        0     3552 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/openram/sram-cache-gen.py
--rw-r--r--   0        0        0     5531 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/openram/sram-cache.json
--rw-r--r--   0        0        0      172 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/openram/srams.txt
--rw-r--r--   0        0        0      785 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/setRC.tcl
--rw-r--r--   0        0        0      421 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning.json
--rw-r--r--   0        0        0     1005 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json
--rw-r--r--   0        0        0     1597 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json
--rw-r--r--   0        0        0      114 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/sites.json
--rwxr-xr-x   0        0        0     3221 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py
--rw-r--r--   0        0        0     2274 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json
--rwxr-xr-x   0        0        0     3259 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen.py
--rw-r--r--   0        0        0     2478 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130_lefpin.map
--rwxr-xr-x   0        0        0     3010 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sram22/sram-cache-gen.py
--rw-r--r--   0        0        0     6699 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sram22/sram-cache.json
--rw-r--r--   0        0        0      320 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sram22/srams.txt
--rw-r--r--   0        0        0    16216 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/sky130.tech.json
--rw-r--r--   0        0        0     6699 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/sram-cache.json
--rw-r--r--   0        0        0    10942 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/sky130/sram_compiler/__init__.py
--rw-r--r--   0        0        0      330 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/vivado/vivado.plsi_config.json
--rw-r--r--   0        0        0      456 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/technology/vivado/vivado.tech.json
--rw-r--r--   0        0        0    12224 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/timing/tempus/__init__.py
--rw-r--r--   0        0        0      605 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/timing/tempus/defaults.yml
--rw-r--r--   0        0        0    14969 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/utils/__init__.py
--rw-r--r--   0        0        0     3300 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/utils/lef_utils.py
--rw-r--r--   0        0        0     1844 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/utils/verilog_utils.py
--rw-r--r--   0        0        0      398 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/__init__.py
--rw-r--r--   0        0        0    92096 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/cli_driver.py
--rw-r--r--   0        0        0    34891 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/constraints.py
--rw-r--r--   0        0        0    84324 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/driver.py
--rw-r--r--   0        0        0    29715 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/hammer_build_systems.py
--rw-r--r--   0        0        0    75866 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/hammer_tool.py
--rw-r--r--   0        0        0    97300 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/hammer_vlsi_impl.py
--rw-r--r--   0        0        0     1655 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/hooks.py
--rw-r--r--   0        0        0    10265 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/submit_command.py
--rw-r--r--   0        0        0    10163 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/units.py
--rw-r--r--   0        0        0       61 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/vendor/__init__.py
--rw-r--r--   0        0        0     6349 2023-03-20 22:33:21.818223 hammer_vlsi-1.1.0/hammer/vlsi/vendor/def2stream.py
--rw-r--r--   0        0        0    12189 2023-03-20 22:33:21.822223 hammer_vlsi-1.1.0/hammer/vlsi/vendor/openroad.py
--rw-r--r--   0        0        0     2343 2023-03-20 22:34:15.862919 hammer_vlsi-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10009 1970-01-01 00:00:00.000000 hammer_vlsi-1.1.0/setup.py
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 hammer_vlsi-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1568 2023-04-20 22:26:21.684385 hammer_vlsi-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2297 2023-04-20 22:26:21.684385 hammer_vlsi-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/__init__.py
+-rw-r--r--   0        0        0    20617 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/cadence/__init__.py
+-rw-r--r--   0        0        0      436 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/cadence/defaults.yml
+-rw-r--r--   0        0        0      456 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/cadence/defaults_types.yml
+-rw-r--r--   0        0        0        0 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/mentor/__init__.py
+-rw-r--r--   0        0        0      571 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/mentor/defaults.yml
+-rw-r--r--   0        0        0      600 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/mentor/defaults_types.yml
+-rw-r--r--   0        0        0        0 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/openroad/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/openroad/defaults.yml
+-rw-r--r--   0        0        0      207 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/openroad/defaults_types.yml
+-rw-r--r--   0        0        0     3592 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/synopsys/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/synopsys/defaults.yml
+-rw-r--r--   0        0        0      415 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/synopsys/defaults_types.yml
+-rw-r--r--   0        0        0     3653 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/vivado/vivado_core.py
+-rw-r--r--   0        0        0      147 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/builtins.yml
+-rw-r--r--   0        0        0       81 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/common.py
+-rw-r--r--   0        0        0    51427 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/config_src.py
+-rw-r--r--   0        0        0    46353 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/defaults.yml
+-rw-r--r--   0        0        0    18317 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/defaults_types.yml
+-rw-r--r--   0        0        0     3904 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/yaml2json.py
+-rw-r--r--   0        0        0     1467 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/icv/README.md
+-rw-r--r--   0        0        0     7030 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/icv/__init__.py
+-rw-r--r--   0        0        0     1305 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/icv/defaults.yml
+-rw-r--r--   0        0        0     6551 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/magic/__init__.py
+-rw-r--r--   0        0        0      617 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/magic/defaults.yml
+-rw-r--r--   0        0        0      516 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/mockdrc/__init__.py
+-rw-r--r--   0        0        0      421 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/nop/__init__.py
+-rw-r--r--   0        0        0     4221 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/openroad/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/openroad/defaults.yml
+-rw-r--r--   0        0        0    11337 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/formal/conformal/__init__.py
+-rw-r--r--   0        0        0      963 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/formal/conformal/defaults.yml
+-rwxr-xr-x   0        0        0    16492 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/generate_properties.py
+-rw-r--r--   0        0        0      251 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/logging/__init__.py
+-rw-r--r--   0        0        0     8650 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/logging/logging.py
+-rw-r--r--   0        0        0     2033 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/logging/test.py
+-rw-r--r--   0        0        0     9013 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/icv/__init__.py
+-rw-r--r--   0        0        0     1454 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/icv/defaults.yml
+-rw-r--r--   0        0        0      600 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/mocklvs/__init__.py
+-rw-r--r--   0        0        0     8263 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/netgen/__init__.py
+-rw-r--r--   0        0        0      628 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/netgen/defaults.yml
+-rw-r--r--   0        0        0      480 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/nop/__init__.py
+-rw-r--r--   0        0        0    56234 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/innovus/__init__.py
+-rw-r--r--   0        0        0     1681 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/innovus/defaults.yml
+-rw-r--r--   0        0        0     2510 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/innovus/dump_stackup_to_json.tcl
+-rw-r--r--   0        0        0     3461 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/mockpar/__init__.py
+-rw-r--r--   0        0        0       77 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/mockpar/defaults.yml
+-rw-r--r--   0        0        0      966 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/nop/__init__.py
+-rw-r--r--   0        0        0     4816 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/openroad/README.md
+-rw-r--r--   0        0        0    85243 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/openroad/__init__.py
+-rw-r--r--   0        0        0     4727 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/openroad/defaults.yml
+-rw-r--r--   0        0        0     1155 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/openroad/defaults_types.yml
+-rw-r--r--   0        0        0     1926 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/vivado/__init__.py
+-rw-r--r--   0        0        0    13460 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/pcb/generic/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/pcb/generic/defaults.yml
+-rw-r--r--   0        0        0     9710 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/joules/__init__.py
+-rw-r--r--   0        0        0      450 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/joules/defaults.yml
+-rw-r--r--   0        0        0    41055 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/voltus/__init__.py
+-rw-r--r--   0        0        0     1187 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/voltus/defaults.yml
+-rw-r--r--   0        0        0        0 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/py.typed
+-rw-r--r--   0        0        0     1723 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/get_config.py
+-rw-r--r--   0        0        0     3538 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/hammer_generate_mdf.py
+-rw-r--r--   0        0        0      147 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/hammer_shell_test.py
+-rw-r--r--   0        0        0      188 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/hammer_vlsi.py
+-rw-r--r--   0        0        0      691 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/readlink_array.py
+-rw-r--r--   0        0        0     1532 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/yaml2json.py
+-rw-r--r--   0        0        0     1324 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/mocksim/__init__.py
+-rw-r--r--   0        0        0       76 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/mocksim/defaults.yml
+-rw-r--r--   0        0        0    17431 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/vcs/__init__.py
+-rw-r--r--   0        0        0      699 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/vcs/defaults.yml
+-rw-r--r--   0        0        0    19752 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/xcelium/__init__.py
+-rw-r--r--   0        0        0     1332 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults.yml
+-rw-r--r--   0        0        0      804 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults_types.yml
+-rw-r--r--   0        0        0      701 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sram_generator/mocksram_generator/__init__.py
+-rw-r--r--   0        0        0      470 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sram_generator/nop/__init__.py
+-rw-r--r--   0        0        0    18000 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/genus/__init__.py
+-rw-r--r--   0        0        0      524 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/genus/defaults.yml
+-rw-r--r--   0        0        0     2352 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/mocksynth/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/mocksynth/defaults.yml
+-rw-r--r--   0        0        0      354 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/nop/__init__.py
+-rw-r--r--   0        0        0     2467 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/__init__.py
+-rw-r--r--   0        0        0      899 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/defaults.yml
+-rw-r--r--   0        0        0      144 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/board.tcl
+-rw-r--r--   0        0        0     1419 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/init.tcl
+-rw-r--r--   0        0        0      749 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/ip.tcl
+-rw-r--r--   0        0        0      360 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/mcs.tcl
+-rw-r--r--   0        0        0      247 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/msg.tcl
+-rw-r--r--   0        0        0     1847 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/par.tcl
+-rw-r--r--   0        0        0      342 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/paths.tcl
+-rw-r--r--   0        0        0      426 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/project.tcl
+-rw-r--r--   0        0        0     1291 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/prologue.tcl
+-rwxr-xr-x   0        0        0      226 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/run-par
+-rwxr-xr-x   0        0        0      189 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/run-synthesis
+-rw-r--r--   0        0        0      291 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/syn.tcl
+-rw-r--r--   0        0        0       26 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/vc707.xdc
+-rw-r--r--   0        0        0      183 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/vivado_setup.sh
+-rw-r--r--   0        0        0    14891 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/yosys/__init__.py
+-rw-r--r--   0        0        0      630 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults.yml
+-rw-r--r--   0        0        0      594 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults_types.yml
+-rw-r--r--   0        0        0    59569 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/tech/__init__.py
+-rw-r--r--   0        0        0      921 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/tech/specialcells.py
+-rw-r--r--   0        0        0    18266 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/tech/stackup.py
+-rw-r--r--   0        0        0     4117 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/README.md
+-rw-r--r--   0        0        0    13924 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/__init__.py
+-rw-r--r--   0        0        0    47808 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/asap7.tech.json
+-rw-r--r--   0        0        0     1450 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/calibre.layerprops
+-rw-r--r--   0        0        0     3488 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/defaults.yml
+-rw-r--r--   0        0        0      155 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/defaults_types.yml
+-rwxr-xr-x   0        0        0     4305 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/gds_scale.py
+-rw-r--r--   0        0        0      314 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/latch_map.v
+-rw-r--r--   0        0        0      657 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/lefdefLayer.map
+-rwxr-xr-x   0        0        0     3622 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache-gen.py
+-rw-r--r--   0        0        0    54410 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache.json
+-rw-r--r--   0        0        0     7899 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/__init__.py
+-rw-r--r--   0        0        0    10084 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds
+-rw-r--r--   0        0        0    10784 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds
+-rw-r--r--   0        0        0    17108 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds
+-rw-r--r--   0        0        0    19564 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds
+-rw-r--r--   0        0        0    19916 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds
+-rw-r--r--   0        0        0    22376 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds
+-rw-r--r--   0        0        0    31156 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds
+-rw-r--r--   0        0        0     6580 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds
+-rw-r--r--   0        0        0     7806 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds
+-rw-r--r--   0        0        0     8510 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds
+-rw-r--r--   0        0        0    12022 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds
+-rw-r--r--   0        0        0    20098 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds
+-rw-r--r--   0        0        0    22558 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds
+-rw-r--r--   0        0        0    23610 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds
+-rw-r--r--   0        0        0    30634 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds
+-rw-r--r--   0        0        0     6054 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds
+-rw-r--r--   0        0        0     6756 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds
+-rw-r--r--   0        0        0    58904 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds
+-rw-r--r--   0        0        0    16760 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds
+-rw-r--r--   0        0        0    23080 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds
+-rw-r--r--   0        0        0    23784 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds
+-rw-r--r--   0        0        0    30808 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds
+-rw-r--r--   0        0        0     6228 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds
+-rw-r--r--   0        0        0    23962 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds
+-rw-r--r--   0        0        0    10784 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds
+-rw-r--r--   0        0        0     7280 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds
+-rw-r--r--   0        0        0    59078 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds
+-rw-r--r--   0        0        0    16934 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds
+-rw-r--r--   0        0        0    30982 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds
+-rw-r--r--   0        0        0     6402 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds
+-rw-r--r--   0        0        0    58556 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds
+-rw-r--r--   0        0        0    11140 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds
+-rw-r--r--   0        0        0    11492 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds
+-rw-r--r--   0        0        0    11844 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds
+-rw-r--r--   0        0        0    16408 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds
+-rw-r--r--   0        0        0    17112 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds
+-rw-r--r--   0        0        0     5880 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds
+-rw-r--r--   0        0        0    18918 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds
+-rw-r--r--   0        0        0    32966 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds
+-rw-r--r--   0        0        0     8378 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds
+-rw-r--r--   0        0        0    11890 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds
+-rw-r--r--   0        0        0    17858 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds
+-rw-r--r--   0        0        0    31906 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds
+-rw-r--r--   0        0        0     7322 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds
+-rw-r--r--   0        0        0    10834 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds
+-rw-r--r--   0        0        0    18210 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds
+-rw-r--r--   0        0        0    23478 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds
+-rw-r--r--   0        0        0    32258 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds
+-rw-r--r--   0        0        0    32962 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds
+-rw-r--r--   0        0        0    38230 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds
+-rw-r--r--   0        0        0     7674 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds
+-rw-r--r--   0        0        0    11186 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds
+-rw-r--r--   0        0        0    18562 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds
+-rw-r--r--   0        0        0    25586 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds
+-rw-r--r--   0        0        0    32610 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds
+-rw-r--r--   0        0        0     8026 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds
+-rw-r--r--   0        0        0    11538 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds
+-rw-r--r--   0        0        0     7051 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef
+-rw-r--r--   0        0        0     7398 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef
+-rw-r--r--   0        0        0    11742 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef
+-rw-r--r--   0        0        0    13264 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef
+-rw-r--r--   0        0        0    13537 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef
+-rw-r--r--   0        0        0    15249 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef
+-rw-r--r--   0        0        0    21091 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef
+-rw-r--r--   0        0        0     4754 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef
+-rw-r--r--   0        0        0     5494 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef
+-rw-r--r--   0        0        0     6031 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef
+-rw-r--r--   0        0        0     8355 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef
+-rw-r--r--   0        0        0    13650 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef
+-rw-r--r--   0        0        0    15362 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef
+-rw-r--r--   0        0        0    15985 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef
+-rw-r--r--   0        0        0    20654 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef
+-rw-r--r--   0        0        0     4352 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef
+-rw-r--r--   0        0        0     4888 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef
+-rw-r--r--   0        0        0    39648 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef
+-rw-r--r--   0        0        0    11450 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef
+-rw-r--r--   0        0        0    15574 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef
+-rw-r--r--   0        0        0    16119 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef
+-rw-r--r--   0        0        0    20788 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef
+-rw-r--r--   0        0        0     4484 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef
+-rw-r--r--   0        0        0    16251 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef
+-rw-r--r--   0        0        0     7417 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef
+-rw-r--r--   0        0        0     5107 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef
+-rw-r--r--   0        0        0    39781 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef
+-rw-r--r--   0        0        0    11583 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef
+-rw-r--r--   0        0        0    20958 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef
+-rw-r--r--   0        0        0     4611 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef
+-rw-r--r--   0        0        0    39308 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef
+-rw-r--r--   0        0        0     7675 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef
+-rw-r--r--   0        0        0     7946 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef
+-rw-r--r--   0        0        0     8218 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef
+-rw-r--r--   0        0        0    11176 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef
+-rw-r--r--   0        0        0    11716 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef
+-rw-r--r--   0        0        0     4218 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef
+-rw-r--r--   0        0        0    12982 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef
+-rw-r--r--   0        0        0    22452 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef
+-rw-r--r--   0        0        0     5940 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef
+-rw-r--r--   0        0        0     8262 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef
+-rw-r--r--   0        0        0    12165 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef
+-rw-r--r--   0        0        0    21631 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef
+-rw-r--r--   0        0        0     5123 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef
+-rw-r--r--   0        0        0     7446 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef
+-rw-r--r--   0        0        0    12437 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef
+-rw-r--r--   0        0        0    15987 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef
+-rw-r--r--   0        0        0    21899 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef
+-rw-r--r--   0        0        0    22455 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef
+-rw-r--r--   0        0        0    26004 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef
+-rw-r--r--   0        0        0     5403 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef
+-rw-r--r--   0        0        0     7718 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef
+-rw-r--r--   0        0        0    12708 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef
+-rw-r--r--   0        0        0    17441 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef
+-rw-r--r--   0        0        0    22174 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef
+-rw-r--r--   0        0        0     5670 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef
+-rw-r--r--   0        0        0     7988 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef
+-rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15401 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15267 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15364 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15186 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15435 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15305 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15394 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15242 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15198 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15046 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15345 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15211 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15504 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15294 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15495 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15285 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15372 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15363 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15267 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15363 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15267 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15354 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15258 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15386 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15224 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15368 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15206 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28859 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28513 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28859 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28513 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28846 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28500 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28846 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28500 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28793 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28447 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28793 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28447 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28602 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28256 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28780 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28434 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28792 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28534 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28792 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28534 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28869 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28555 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28869 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28555 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28869 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28555 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28856 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28542 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28856 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28542 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0      773 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/srams.txt
+-rw-r--r--   0        0        0      576 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/README.md
+-rw-r--r--   0        0        0      365 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/__init__.py
+-rw-r--r--   0        0        0      952 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/defaults.yml
+-rw-r--r--   0        0        0     5912 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/nangate45.tech.json
+-rw-r--r--   0        0        0     1554 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/sram-cache.json
+-rw-r--r--   0        0        0     2835 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/sram_compiler/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nop/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nop/defaults.yml
+-rw-r--r--   0        0        0       82 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nop/nop.tech.json
+-rw-r--r--   0        0        0     6649 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/README.md
+-rw-r--r--   0        0        0    14127 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/__init__.py
+-rw-r--r--   0        0        0     5035 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/defaults.yml
+-rw-r--r--   0        0        0      711 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/defaults_types.yml
+-rw-r--r--   0        0        0      899 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells-gen.py
+-rw-r--r--   0        0        0    11554 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells.txt
+-rw-r--r--   0        0        0     2907 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/fill.json
+-rwxr-xr-x   0        0        0     3552 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache-gen.py
+-rw-r--r--   0        0        0     5531 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache.json
+-rw-r--r--   0        0        0      172 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/srams.txt
+-rw-r--r--   0        0        0      785 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/setRC.tcl
+-rw-r--r--   0        0        0      421 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning.json
+-rw-r--r--   0        0        0     1005 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json
+-rw-r--r--   0        0        0     1597 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json
+-rw-r--r--   0        0        0      114 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/sites.json
+-rwxr-xr-x   0        0        0     3221 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py
+-rw-r--r--   0        0        0     2274 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json
+-rwxr-xr-x   0        0        0     3259 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen.py
+-rw-r--r--   0        0        0     2478 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130_lefpin.map
+-rwxr-xr-x   0        0        0     3010 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache-gen.py
+-rw-r--r--   0        0        0     6699 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache.json
+-rw-r--r--   0        0        0      320 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/srams.txt
+-rw-r--r--   0        0        0    16216 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/sky130.tech.json
+-rw-r--r--   0        0        0     6699 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/sram-cache.json
+-rw-r--r--   0        0        0    10942 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/sram_compiler/__init__.py
+-rw-r--r--   0        0        0      330 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/vivado/vivado.plsi_config.json
+-rw-r--r--   0        0        0      456 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/vivado/vivado.tech.json
+-rw-r--r--   0        0        0    12224 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/timing/tempus/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/timing/tempus/defaults.yml
+-rw-r--r--   0        0        0    14969 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/utils/__init__.py
+-rw-r--r--   0        0        0     3300 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/utils/lef_utils.py
+-rw-r--r--   0        0        0     1844 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/utils/verilog_utils.py
+-rw-r--r--   0        0        0      398 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/__init__.py
+-rw-r--r--   0        0        0    92096 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/cli_driver.py
+-rw-r--r--   0        0        0    34891 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/constraints.py
+-rw-r--r--   0        0        0    84324 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/driver.py
+-rw-r--r--   0        0        0    29715 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hammer_build_systems.py
+-rw-r--r--   0        0        0    75866 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hammer_tool.py
+-rw-r--r--   0        0        0    99097 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hammer_vlsi_impl.py
+-rw-r--r--   0        0        0     1655 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hooks.py
+-rw-r--r--   0        0        0    10265 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/submit_command.py
+-rw-r--r--   0        0        0    10163 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/units.py
+-rw-r--r--   0        0        0       61 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/vendor/__init__.py
+-rw-r--r--   0        0        0     6349 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/vendor/def2stream.py
+-rw-r--r--   0        0        0    12189 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/vendor/openroad.py
+-rw-r--r--   0        0        0     2343 2023-04-20 22:27:13.501184 hammer_vlsi-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10009 1970-01-01 00:00:00.000000 hammer_vlsi-1.1.1/setup.py
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 hammer_vlsi-1.1.1/PKG-INFO
```

### Comparing `hammer_vlsi-1.1.0/LICENSE` & `hammer_vlsi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/README.md` & `hammer_vlsi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/common/cadence/__init__.py` & `hammer_vlsi-1.1.1/hammer/common/cadence/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/common/mentor/defaults.yml` & `hammer_vlsi-1.1.1/hammer/common/mentor/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/common/mentor/defaults_types.yml` & `hammer_vlsi-1.1.1/hammer/common/mentor/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/common/synopsys/__init__.py` & `hammer_vlsi-1.1.1/hammer/common/synopsys/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/common/vivado/vivado_core.py` & `hammer_vlsi-1.1.1/hammer/common/vivado/vivado_core.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/config/config_src.py` & `hammer_vlsi-1.1.1/hammer/config/config_src.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/config/defaults.yml` & `hammer_vlsi-1.1.1/hammer/config/defaults.yml`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
   #        including vlsi.inputs.supplies.
   # manual - Use the value given in power_spec_contents with type given in power_spec_type
   # empty - Do not use any power specification
   power_spec_type: null # Optional: Power specification type. (str)
   # Specifies what kind/version/type of power specification to use
   # Valid options:
   # cpf - Use the common power format commonly used in Cadence tools
-  # upf - Use the universal power format, IEEE 1801-2015
+  # upf - Use the universal power format, IEEE 1801-2009
   power_spec_contents: null # Optional: Contents of a power specification in the above type (str)
 
   sram_parameters: [] # SRAM Parameters
 
   bumps_mode: empty # Bumps settings mode. (str)
   # Specifies how to setup the bumps for your design.
   # Currently only support rectangular, evenly-spaced grids
```

### Comparing `hammer_vlsi-1.1.0/hammer/config/defaults_types.yml` & `hammer_vlsi-1.1.1/hammer/config/defaults_types.yml`

 * *Files 2% similar despite different names*

```diff
@@ -104,27 +104,27 @@
     # Manual hierarchical constraints. Overrides generic constraints on a per module basis.
     constraints: list[dict[str, list]]
 
   # ILMs for hierarchical mode.
   ilms: list[dict[str, str]]
 
   # Multi-mode multi-corner setups, overrides supplies
-  mmmc_corners: list[dict[str, str]]
+  mmmc_corners: list[dict[str, Any]]
 
   # Clock ports of the top-level module.
-  clocks: list[dict[str, str]]
+  clocks: list[dict[str, Any]]
 
   # Default output pin load capacitance.
   default_output_load: int
 
   # List of output load constraints.
   output_loads: list[dict[str, str]]
 
   # List of delay constraints.
-  delays: list[dict[str, str]]
+  delays: list[dict[str, Any]]
 
   # List of custom sdc constraints to use. (List[str])
   custom_sdc_constraints: list[str]
 
   # List of placement constraints for floorplanning.
   placement_constraints: list[dict[str, Any]]
 
@@ -157,31 +157,31 @@
     # global_x_offset (float) - offset the bump map in the x-axis 
     global_x_offset: float
     # global_y_offset (float) - offset the bump map in the y-axis 
     global_y_offset: float
     # cell (str) - Name of the default bump cell
     cell: str
     # assignments - List of BumpAssignment structs. You must specify one of name or no_connect.
-    assignments: list[dict[str, str]]
+    assignments: list[dict[str, Any]]
 
   # Naming scheme for the bumps' actual physical pin designators
   # type: str
   bumps_pin_naming_scheme: str
 
   # Pin placement mode. (str)
   pin_mode: str
   pin:
     # Pin generation modes.
     generate_mode: str
 
     # List of PinAssignment Structs.
-    assignments: list[dict[str, str]]
+    assignments: list[dict[str, Any]]
 
   # List of decap constraints (DecapConstraint struct).
-  decaps: list[dict[str, str]]
+  decaps: list[dict[str, Any]]
 
   # SVG visualization of placement constraints and bumps for the current hierarchical module.
   visualization:
     # Type of visualization to draw
     # type: str
     mode: str
     # Name of the desired output SVG file
@@ -353,15 +353,15 @@
   # Input layout file
   layout_file: Optional[str]
 
   # Input list of schematic files
   schematic_files: list[str]
 
   # Input list of ILMStructs
-  ilms: list[str]
+  ilms: list[dict[str, Any]]
 
   # Input list of Hcells
   hcells_list: list[str]
 
   # Valid modes are auto, manual, prepend, and append
   additional_lvs_text_mode: str
   # Custom LVS command text to add after the boilerplate commands at the top of the run file
```

### Comparing `hammer_vlsi-1.1.0/hammer/config/yaml2json.py` & `hammer_vlsi-1.1.1/hammer/config/yaml2json.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/drc/icv/README.md` & `hammer_vlsi-1.1.1/hammer/drc/icv/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/drc/icv/__init__.py` & `hammer_vlsi-1.1.1/hammer/drc/icv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             layerprops_file = self.get_setting("synopsys.layerprops")
             if layerprops_file is not None:
                 f.writelines(l for l in open(layerprops_file))
 
         with open(self.view_drc_script, "w") as f:
             f.write("""
         cd {run_dir}
-        source enter
+        source ./enter
         # Start Synopsys IC Validator WorkBench and wait for port to open before starting VUE
         {icvwb} -socket {port} -run {macrofile} {gds} &
         while ! nc -z localhost {port}; do
             sleep 0.1
         done
         {icv_vue} -64 -load {results} -lay icwb -layArgs Port {port}
             """.format(
@@ -140,15 +140,15 @@
             assert isinstance(include_dirs, list)
             if len(include_dirs) > 0:
                 f.write(" -I " + " -I ".join(include_dirs))
 
             # Config runset file
             config_rs = self.get_setting("drc.icv.config_runset")  # type: Optional[str]
             if config_rs is not None:
-                f.write(" -config_runset" + config_rs)
+                f.write(" -runset_config " + config_rs)
         return True
 
     @property
     def generated_scripts_dir(self) -> str:
         return os.path.join(self.run_dir, "generated-scripts")
 
     @property
```

### Comparing `hammer_vlsi-1.1.0/hammer/drc/icv/defaults.yml` & `hammer_vlsi-1.1.1/hammer/drc/icv/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/drc/magic/__init__.py` & `hammer_vlsi-1.1.1/hammer/drc/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/drc/magic/defaults.yml` & `hammer_vlsi-1.1.1/hammer/drc/magic/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/drc/mockdrc/__init__.py` & `hammer_vlsi-1.1.1/hammer/drc/mockdrc/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/drc/openroad/__init__.py` & `hammer_vlsi-1.1.1/hammer/drc/openroad/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/formal/conformal/__init__.py` & `hammer_vlsi-1.1.1/hammer/formal/conformal/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/formal/conformal/defaults.yml` & `hammer_vlsi-1.1.1/hammer/formal/conformal/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/generate_properties.py` & `hammer_vlsi-1.1.1/hammer/generate_properties.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/logging/logging.py` & `hammer_vlsi-1.1.1/hammer/logging/logging.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/logging/test.py` & `hammer_vlsi-1.1.1/hammer/logging/test.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/lvs/icv/__init__.py` & `hammer_vlsi-1.1.1/hammer/lvs/icv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             layerprops_file = self.get_setting("synopsys.layerprops")
             if layerprops_file is not None:
                 f.writelines(l for l in open(layerprops_file))
 
         with open(self.view_lvs_script, "w") as f:
             f.write("""
         cd {run_dir}
-        source enter
+        source ./enter
         # Start Synopsys IC Validator WorkBench and wait for port to open before starting VUE
         {icvwb} -socket {port} -run {macrofile} {gds} &
         while ! nc -z localhost {port}; do
             sleep 0.1
         done
         {icv_vue} -64 -load {results} -lay icwb -layArgs Port {port}
             """.format(
@@ -178,17 +178,17 @@
             # Preprocessor directories to include
             include_dirs = self.get_setting("lvs.icv.include_dirs")  # type: List[str]
             assert isinstance(include_dirs, list)
             if len(include_dirs) > 0:
                 f.write(" -I " + " -I ".join(include_dirs))
 
             # Config runset file
-            config_rs = self.get_setting("drc.icv.config_runset")  # type: Optional[str]
+            config_rs = self.get_setting("lvs.icv.config_runset")  # type: Optional[str]
             if config_rs is not None:
-                f.write(" -config_runset" + config_rs)
+                f.write(" -runset_config " + config_rs)
         return True
 
     @property
     def generated_scripts_dir(self) -> str:
         return os.path.join(self.run_dir, "generated-scripts")
 
     @property
```

### Comparing `hammer_vlsi-1.1.0/hammer/lvs/icv/defaults.yml` & `hammer_vlsi-1.1.1/hammer/lvs/icv/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/lvs/mocklvs/__init__.py` & `hammer_vlsi-1.1.1/hammer/lvs/mocklvs/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/lvs/netgen/__init__.py` & `hammer_vlsi-1.1.1/hammer/lvs/netgen/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/lvs/netgen/defaults.yml` & `hammer_vlsi-1.1.1/hammer/lvs/netgen/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/innovus/__init__.py` & `hammer_vlsi-1.1.1/hammer/par/innovus/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/innovus/defaults.yml` & `hammer_vlsi-1.1.1/hammer/par/innovus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/innovus/dump_stackup_to_json.tcl` & `hammer_vlsi-1.1.1/hammer/par/innovus/dump_stackup_to_json.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/mockpar/__init__.py` & `hammer_vlsi-1.1.1/hammer/par/mockpar/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/nop/__init__.py` & `hammer_vlsi-1.1.1/hammer/par/nop/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/openroad/README.md` & `hammer_vlsi-1.1.1/hammer/par/openroad/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/openroad/__init__.py` & `hammer_vlsi-1.1.1/hammer/par/openroad/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/openroad/defaults.yml` & `hammer_vlsi-1.1.1/hammer/par/openroad/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/openroad/defaults_types.yml` & `hammer_vlsi-1.1.1/hammer/par/openroad/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/par/vivado/__init__.py` & `hammer_vlsi-1.1.1/hammer/par/vivado/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/pcb/generic/__init__.py` & `hammer_vlsi-1.1.1/hammer/pcb/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/pcb/generic/defaults.yml` & `hammer_vlsi-1.1.1/hammer/pcb/generic/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/power/joules/__init__.py` & `hammer_vlsi-1.1.1/hammer/power/joules/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/power/voltus/__init__.py` & `hammer_vlsi-1.1.1/hammer/power/voltus/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/power/voltus/defaults.yml` & `hammer_vlsi-1.1.1/hammer/power/voltus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/shell/get_config.py` & `hammer_vlsi-1.1.1/hammer/shell/get_config.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/shell/hammer_generate_mdf.py` & `hammer_vlsi-1.1.1/hammer/shell/hammer_generate_mdf.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/shell/readlink_array.py` & `hammer_vlsi-1.1.1/hammer/shell/readlink_array.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/shell/yaml2json.py` & `hammer_vlsi-1.1.1/hammer/shell/yaml2json.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/sim/mocksim/__init__.py` & `hammer_vlsi-1.1.1/hammer/sim/mocksim/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/sim/vcs/__init__.py` & `hammer_vlsi-1.1.1/hammer/sim/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/sim/vcs/defaults.yml` & `hammer_vlsi-1.1.1/hammer/sim/vcs/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/sim/xcelium/__init__.py` & `hammer_vlsi-1.1.1/hammer/sim/xcelium/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/sim/xcelium/defaults.yml` & `hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/sim/xcelium/defaults_types.yml` & `hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/sram_generator/mocksram_generator/__init__.py` & `hammer_vlsi-1.1.1/hammer/sram_generator/mocksram_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/genus/__init__.py` & `hammer_vlsi-1.1.1/hammer/synthesis/genus/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/genus/defaults.yml` & `hammer_vlsi-1.1.1/hammer/synthesis/genus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/mocksynth/__init__.py` & `hammer_vlsi-1.1.1/hammer/synthesis/mocksynth/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/vivado/__init__.py` & `hammer_vlsi-1.1.1/hammer/synthesis/vivado/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/vivado/defaults.yml` & `hammer_vlsi-1.1.1/hammer/synthesis/vivado/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/init.tcl` & `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/init.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/ip.tcl` & `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/ip.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/par.tcl` & `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/par.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/vivado/file_templates/prologue.tcl` & `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/prologue.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/yosys/__init__.py` & `hammer_vlsi-1.1.1/hammer/synthesis/yosys/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/yosys/defaults.yml` & `hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/synthesis/yosys/defaults_types.yml` & `hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/tech/__init__.py` & `hammer_vlsi-1.1.1/hammer/tech/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/tech/specialcells.py` & `hammer_vlsi-1.1.1/hammer/tech/specialcells.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/tech/stackup.py` & `hammer_vlsi-1.1.1/hammer/tech/stackup.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/README.md` & `hammer_vlsi-1.1.1/hammer/technology/asap7/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/__init__.py` & `hammer_vlsi-1.1.1/hammer/technology/asap7/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/asap7.tech.json` & `hammer_vlsi-1.1.1/hammer/technology/asap7/asap7.tech.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/calibre.layerprops` & `hammer_vlsi-1.1.1/hammer/technology/asap7/calibre.layerprops`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/defaults.yml` & `hammer_vlsi-1.1.1/hammer/technology/asap7/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/gds_scale.py` & `hammer_vlsi-1.1.1/hammer/technology/asap7/gds_scale.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/lefdefLayer.map` & `hammer_vlsi-1.1.1/hammer/technology/asap7/lefdefLayer.map`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram-cache-gen.py` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram-cache.json` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/__init__.py` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/asap7/srams.txt` & `hammer_vlsi-1.1.1/hammer/technology/asap7/srams.txt`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/nangate45/README.md` & `hammer_vlsi-1.1.1/hammer/technology/nangate45/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/nangate45/defaults.yml` & `hammer_vlsi-1.1.1/hammer/technology/nangate45/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/nangate45/nangate45.tech.json` & `hammer_vlsi-1.1.1/hammer/technology/nangate45/nangate45.tech.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/nangate45/sram-cache.json` & `hammer_vlsi-1.1.1/hammer/technology/nangate45/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/nangate45/sram_compiler/__init__.py` & `hammer_vlsi-1.1.1/hammer/technology/nangate45/sram_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/README.md` & `hammer_vlsi-1.1.1/hammer/technology/sky130/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/__init__.py` & `hammer_vlsi-1.1.1/hammer/technology/sky130/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/defaults.yml` & `hammer_vlsi-1.1.1/hammer/technology/sky130/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/defaults_types.yml` & `hammer_vlsi-1.1.1/hammer/technology/sky130/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/cells-gen.py` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/cells.txt` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells.txt`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/fill.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/fill.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/openram/sram-cache-gen.py` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/openram/sram-cache.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/setRC.tcl` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/setRC.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130-tech-gen.py` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sky130_lefpin.map` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130_lefpin.map`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sram22/sram-cache-gen.py` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/extra/sram22/sram-cache.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/sky130.tech.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/sky130.tech.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/sram-cache.json` & `hammer_vlsi-1.1.1/hammer/technology/sky130/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/technology/sky130/sram_compiler/__init__.py` & `hammer_vlsi-1.1.1/hammer/technology/sky130/sram_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/timing/tempus/__init__.py` & `hammer_vlsi-1.1.1/hammer/timing/tempus/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/timing/tempus/defaults.yml` & `hammer_vlsi-1.1.1/hammer/timing/tempus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/utils/__init__.py` & `hammer_vlsi-1.1.1/hammer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/utils/lef_utils.py` & `hammer_vlsi-1.1.1/hammer/utils/lef_utils.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/utils/verilog_utils.py` & `hammer_vlsi-1.1.1/hammer/utils/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/cli_driver.py` & `hammer_vlsi-1.1.1/hammer/vlsi/cli_driver.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/constraints.py` & `hammer_vlsi-1.1.1/hammer/vlsi/constraints.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/driver.py` & `hammer_vlsi-1.1.1/hammer/vlsi/driver.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/hammer_build_systems.py` & `hammer_vlsi-1.1.1/hammer/vlsi/hammer_build_systems.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/hammer_tool.py` & `hammer_vlsi-1.1.1/hammer/vlsi/hammer_tool.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/hammer_vlsi_impl.py` & `hammer_vlsi-1.1.1/hammer/vlsi/hammer_vlsi_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -2055,19 +2055,59 @@
         self.attr_setter("_sdf_file", value)
 
 
     ### Outputs ###
     ### END Generated interface HammerTimingTool ###
 
 class HasUPFSupport(HammerTool):
-    """Mix-in trait with functions useful for tools with UPF style power
-    constraints"""
-    @property
-    def upf_power_specification(self) -> str:
-        raise NotImplementedError("Automatic generation of UPF power specifications is not supported yet.")
+   """Mix-in trait with functions useful for tools with UPF style power constraints"""
+   @property
+   def upf_power_specification(self) -> str:
+        output = [] # type: List[str]
+        domain = "AO"
+        #Header
+        output.append('upf_version 2.0')
+        output.append(f'set_design_top {self.top_module}')
+        vdd = VoltageValue(self.get_setting("vlsi.inputs.supplies.VDD"))
+        #Create Single Power Domain
+        output.append(f'create_power_domain {domain} \\')
+        output.append(f'\t-elements {{.}}')
+        #Get Supply Nets
+        power_nets = self.get_all_power_nets() 
+        ground_nets = self.get_all_ground_nets()
+        #Create Supply Ports 
+        for pg_net in (power_nets+ground_nets):
+            if(pg_net.pin != None):
+                #Create Supply Nets
+                output.append(f'create_supply_net {pg_net.name} -domain {domain}')
+                output.append(f'create_supply_port {pg_net.name} -domain {domain} \\')
+                output.append(f'\t-direction in')
+                #Connect Supply Net
+                output.append(f'connect_supply_net {pg_net.name} -ports {pg_net.name}')
+                #Set Domain Supply Net
+        output.append(f'set_domain_supply_net {domain} \\')
+        output.append(f'\t-primary_power_net {power_nets[0].name} \\')
+        output.append(f'\t-primary_ground_net {ground_nets[0].name}')
+        #Add Port States 
+        for p_net in power_nets:
+            if(p_net.pin != None):
+                output.append(f'add_port_state {p_net.name} \\')
+                output.append(f'\t-state {{default {vdd.value}}}')
+        for g_net in ground_nets:
+            if(g_net.pin != None):
+                output.append(f'add_port_state {g_net.name} \\')
+                output.append(f'\t-state {{default 0.0}}')
+        #Create Power State Table
+        output.append('create_pst pwr_state_table \\')
+        output.append(f'\t-supplies {{{" ".join(map(lambda x: x.name, power_nets))} {" ".join(map(lambda x: x.name, ground_nets))}}}')
+        #Add Power States
+        output.append(f'add_pst_state aon \\')
+        output.append(f'\t-pst {{pwr_state_table}} \\')
+        output.append(f'\t-state {{{" ".join(map(lambda x: "default", power_nets+ground_nets))}}}')
+        return "\n".join(output)
 
 
 class HasCPFSupport(HammerTool):
     """Mix-in trait with functions useful for tools with CPF style power
     constraints"""
     @property
     def cpf_power_specification(self) -> str:
@@ -2075,45 +2115,34 @@
         # Just names
         domain = "AO"
         condition = "nominal"
         mode = "aon"
         # Header
         output.append("set_cpf_version 1.0e")
         output.append("set_hierarchy_separator /")
-
-        output.append("set_design {t}".format(t=self.top_module))
-        # Define power and ground nets
+        output.append(f'set_design {self.top_module}')
+        # Define power and ground nets (HARD CODE)
         power_nets = self.get_all_power_nets() # type: List[Supply]
-        ground_nets = self.get_all_ground_nets() # type: List[Supply]
+        ground_nets = self.get_all_ground_nets()# type: List[Supply]
         vdd = VoltageValue(self.get_setting("vlsi.inputs.supplies.VDD")) # type: VoltageValue
-        output.append("create_power_nets -nets {{ {p} }} -voltage {v}".
-                format(p=" ".join(map(lambda x: x.name, power_nets)), v=vdd.value))
-        output.append("create_ground_nets -nets {{ {g} }}".
-                format(g=" ".join(map(lambda x: x.name, ground_nets))))
-
+        output.append(f'create_power_nets -nets {{ {" ".join(map(lambda x: x.name, power_nets))} }} -voltage {vdd.value}')
+        output.append(f'create_ground_nets -nets {{ {" ".join(map(lambda x: x.name, ground_nets))} }}')
         # Define power domain and connections
-        output.append("create_power_domain -name {d} -default".format(d=domain))
+        output.append(f'create_power_domain -name {domain} -default')
         # Assume primary power are first in list
-        output.append("update_power_domain -name {d} -primary_power_net {pp} -primary_ground_net {pg}".
-                format(d=domain, pp=power_nets[0].name, pg=ground_nets[0].name))
+        output.append(f'update_power_domain -name {domain} -primary_power_net {power_nets[0].name} -primary_ground_net {ground_nets[0].name}')
         # Assuming that all power/ground nets correspond to pins
         for pg_net in (power_nets+ground_nets):
             if(pg_net.pin != None):
-                output.append("create_global_connection -domain {d} -net {n} -pins {p}".
-                        format(d=domain, n=pg_net.name, p=pg_net.pin))
-
+                output.append(f'create_global_connection -domain {domain} -net {pg_net.name} -pins {pg_net.pin}')
         # Create nominal operation condtion and power mode
-        output.append("create_nominal_condition -name {c} -voltage {v}".
-                format(c=condition, v=vdd.value))
-        output.append("create_power_mode -name {m} -default -domain_conditions {{{d}@{c}}}".
-                format(m=mode, d=domain, c=condition))
-
+        output.append(f'create_nominal_condition -name {condition} -voltage {vdd.value}')
+        output.append(f'create_power_mode -name {mode} -default -domain_conditions {{{domain}@{condition}}}')
         # Footer
         output.append("end_design")
-
         return "\n".join(output)
 
 class HasSDCSupport(HammerTool):
     """Mix-in trait with functions useful for tools with SDC-style
     constraints."""
     @property
     def sdc_clock_constraints(self) -> str:
```

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/hooks.py` & `hammer_vlsi-1.1.1/hammer/vlsi/hooks.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/submit_command.py` & `hammer_vlsi-1.1.1/hammer/vlsi/submit_command.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/units.py` & `hammer_vlsi-1.1.1/hammer/vlsi/units.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/vendor/def2stream.py` & `hammer_vlsi-1.1.1/hammer/vlsi/vendor/def2stream.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/hammer/vlsi/vendor/openroad.py` & `hammer_vlsi-1.1.1/hammer/vlsi/vendor/openroad.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.0/pyproject.toml` & `hammer_vlsi-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hammer-vlsi"
-version = "1.1.0"
+version = "1.1.1"
 description = "Hammer is a physical design framework that wraps around vendor specific technologies and tools to provide a single API to create ASICs."
 authors = ["Colin Schmidt <colin.schmidt@sifive.com>", "Edward Wang <edward.c.wang@compdigitec.com>", "John Wright <johnwright@eecs.berkeley.edu>"]
 maintainers = ["Harrison Liew <harrisonliew@berkeley.edu>", "Daniel Grubb <dpgrubb@berkeley.edu>"]
 readme = "README.md"
 repository = "https://github.com/ucb-bar/hammer"
 packages = [
     {include = "hammer"}
```

### Comparing `hammer_vlsi-1.1.0/setup.py` & `hammer_vlsi-1.1.1/setup.py`

 * *Files identical despite different names*

```diff
@@ -138,15 +138,15 @@
                      'hammer-shell-test = hammer.shell.hammer_shell_test:main',
                      'hammer-vlsi = hammer.shell.hammer_vlsi:main',
                      'readlink-array = hammer.shell.readlink_array:main',
                      'yaml2json = hammer.shell.yaml2json:main']}
 
 setup_kwargs = {
     'name': 'hammer-vlsi',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Hammer is a physical design framework that wraps around vendor specific technologies and tools to provide a single API to create ASICs.',
     'long_description': "![Logo design by @kenhoberkeley](https://github.com/ucb-bar/hammer/raw/master/doc/logo_transparent.png)\n\n![Hammer PR CI](https://github.com/ucb-bar/hammer/actions/workflows/pr.yml/badge.svg?event=push) ![Hammer publish CI](https://github.com/ucb-bar/hammer/actions/workflows/publish.yml/badge.svg)\n\nHighly Agile Masks Made Effortlessly from RTL (Hammer)\n=============================================\n\nThis is the master (unstable) development branch.\n\nDocumentation\n=============\nThe documentation is found at https://hammer-vlsi.readthedocs.io\nDoc sources are available at `doc/` for offline reading.\n\nHammer currently requires Python 3.9+.\n\nFor a deeper dive into available options and environment configuration:\n\n* [Core Hammer settings](hammer/config/defaults.yml)\n* [Setup documentation](https://hammer-vlsi.readthedocs.io/en/latest/Hammer-Basics/Hammer-Setup.html)\n* [Hammer technology library schema](https://hammer-vlsi.readthedocs.io/en/latest/Technology/Tech-json.html#full-schema)\n* For CAD tool settings, please see the relevant `defaults.yml` for those plugins.\n\nHammer is an integral component of UC Berkeley Architecture Research's [Chipyard framework](https://github.com/ucb-bar/chipyard).\nUseful documentation for how an example block is pushed through the VLSI flow with Hammer in the free ASAP7 and Sky130 PDKs is at https://chipyard.readthedocs.io/en/latest/VLSI.\n\nHistory\n=======\nThe list of contributors can be found in the Git history of the project, or online at https://github.com/ucb-bar/hammer/graphs/contributors\n\nThe Hammer project builds upon the legacy of the PLSI project by Palmer Dabbelt, a previous project which aimed to build a portable VLSI flow. The Hammer project is grateful for the feedback and lessons learned which provided valuable insight that ultimately led to the design and software architecture of Hammer as it is now.\n\nBelow is the list of Hammer publications in reverse chronological order:\n- [Hammer: a modular and reusable physical design flow tool (DAC 2022)](https://dl.acm.org/doi/abs/10.1145/3489517.3530672)\n- [A Methodology for Reusable Physical Design (ISQED 2020)](https://ieeexplore.ieee.org/document/9136999)\n- [PLSI: A Portable VLSI Flow (Master's Thesis, 2017)](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2017/EECS-2017-77.html)\n",
     'author': 'Colin Schmidt',
     'author_email': 'colin.schmidt@sifive.com',
     'maintainer': 'Harrison Liew',
     'maintainer_email': 'harrisonliew@berkeley.edu',
     'url': 'https://github.com/ucb-bar/hammer',
```

### Comparing `hammer_vlsi-1.1.0/PKG-INFO` & `hammer_vlsi-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hammer-vlsi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Hammer is a physical design framework that wraps around vendor specific technologies and tools to provide a single API to create ASICs.
 Home-page: https://github.com/ucb-bar/hammer
 Author: Colin Schmidt
 Author-email: colin.schmidt@sifive.com
 Maintainer: Harrison Liew
 Maintainer-email: harrisonliew@berkeley.edu
 Requires-Python: >=3.9,<4.0
```

