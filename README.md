# TWRP Device Tree for Samsung Galaxy A23 5G (SM-A236M)

The Galaxy A23 5G (codenamed _"a23xq"_) is an upper-mid-range smartphone from Samsung.

It was announced in Augustus 2022 and released in September 2022.

## Device specifications

|                        Feature | Specification                                                                          |
| -----------------------------: | :------------------------------------------------------------------------------------- |
|                        Chipset | Qualcomm SM6375 Snapdragon 695 5G                                                      |
|                            CPU | Octa-core (2x2.2 GHz Kryo 660 Gold, 6x1.7 Ghz Kyro 660 Silver)                         |
|                            GPU | Qualcomm Adreno 619                                                                    |
|                         Memory | 4GB / 6BG / 8GB RAM (LPDDR4X)                                                          |
|                     Shipped OS | Android 12 (One UI 4.1)                                                                |
|                        Storage | 128GB / 256GB (UFS 2.1)                                                                |
|                            SIM | Hybrid Dual SIM (Nano-SIM, dual stand-by)                                              |
|                        MicroSD | Up to 1TB                                                                              |
|                        Battery | 5000mAh Li-Po (non-removable), 25W fast charge                                         |
|                     Dimensions | 165.4 x 76.9 x 8.4 mm (6.51 x 3.03 x 0.33 in)                                          |
|                        Display | 6.6 inches, 104.9 cm2 (~82.5% ratio) 1080 x 2408 pixels, 20:9 ratio (~400 ppi density) |
| Rear Camera 1 (IMX682/S5KGW1P) | 50 MP, f/1.8, (wide), PDAF, OIS                                                        |
|         Rear Camera 2 (S5K3L6) | 5 MP, f/2.2, 123˚ (ultrawide), 1/5.0", 1.12µm                                          |
|         Rear Camera 3 (S5KGW2) | 2 MP, f/2.4, (macro)                                                                   |
|         Rear Camera 4 (S5K3J1) | 2 MP, f/2.4, (depth)                                                                   |
|   Front Camera (IMX616/S5KGD2) | 8 MP, f/2.2, (wide) - International                                                    |
|                    Fingerprint | EFingerprint (side-mounted)                                                            |
|                        Sensors | Accelerometer, Gyro, Proximity (virtual),                                              |

## Device picture

<img src="https://fdn2.gsmarena.com/vv/pics/samsung/galaxy-a23-5g-2.jpg" width="50%"/>

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/LunarStorm97/50ed992.git -b android-12.1 device/samsung/a23xq
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_a23xq-eng
mka recoveryimage
```

## Copyright

```
Copyright (C) 2025 The Android Open Source Project
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
