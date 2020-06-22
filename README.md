# TWRP device tree for Samsung S7 Edge aka hero2lte

 Copyright (C) 2020 Ananjaser1211 Open-source

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.


Add to `.repo/local_manifests/hero2lte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="ananjaser1211/android_device_samsung_hero" path="device/samsung/hero2lte" remote="github" revision="hero2lte" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch omni_hero2lte-eng
mke -j64 recoveryimage
```

Kernel sources are available at: https://github.com/https://github.com/ananjaser1211/Cronos_8890/
