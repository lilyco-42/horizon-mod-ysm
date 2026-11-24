# horizon-mod-ysm (`ysm_models` v3.6.1)

Standalone **Horizon** native mod delivering a 1:1 Rust port of **Yes Steve Model** (`YesSteveModel-Native` + `YesSteveModel`, Apache-2.0).

## Features
- Hierarchical bone-tree renderer (`euler_zyx`, `PoseStack`, `ModelState`, Bedrock `(-X, +Y, -Z)` Euler convention)
- 30-slot `.yanim` player (`idle / walk / run / sneak / jump / ride / swim / extra0..7 / arm.animation.json`)
- Real 3D held-item rendering in both hands (`ThirdPersonRightHand` / `ThirdPersonLeftHand`)
- Horse/vehicle riding detection (`ride` pose) + silky cross-fade blending + left-click swing overlay
- Includes `crates/ysm-native-port` (21/21 unit tests) & CC0 3-color `lyco_ip` model generator

## Build & Install
```bash
horizon-launcher native-build \
  --version nightly-2026-11-20-0a875da \
  --trust-native-code .
```

## Controls
- `Y`: Cycle 3D YSM model
- `G` / `/ysm_play <0..7>`: Switch extra actions
- `W/A/S/D`, `Shift`, `Ctrl`, `Space`, `Left Click`, `Mount Horse`: Automatic animations & 3D held items

Part of the [lilyco-horizon](https://github.com/lilyco-42/lilyco-horizon) ecosystem.
