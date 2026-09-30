# Third-party notices

## Current application builds

Aj Escaño owns the original application materials only. Third-party rights are not transferred or restricted by the proprietary license. Current builds include AndroidX, Kotlin/coroutines, LiteRT LM, the checksum-pinned Qwen3 0.6B INT4 model, and Lora / EB Garamond fonts.

AndroidX and Kotlin use Apache License 2.0. LiteRT and Qwen license and runtime notices are bundled in the app Licenses screen under their original filenames. The fonts use the SIL Open Font License; full notices are included in [lora-OFL.txt](licenses/lora-OFL.txt) and [ebgaramond-OFL.txt](licenses/ebgaramond-OFL.txt), and bundled in the app. Model source and pinned revision/checksum are recorded in `qwen_model/model-manifest.json`.

## Historical Phase 1 notices

The Phase 1 application uses AndroidX (including Jetpack Compose, Material 3, Room, Navigation, Activity, Core and Lifecycle), Kotlin, and Kotlin coroutines, distributed under Apache License 2.0. The license text is included in [licenses/Apache-2.0.txt](licenses/Apache-2.0.txt). Upstream copyright notices remain with their respective authors; AndroidX is developed by the Android Open Source Project and Kotlin/coroutines by JetBrains and contributors.

Gradle and the Android Gradle plugin are build tooling. JUnit, Robolectric, AndroidX Test and Room Testing are test dependencies, not production features. Their license metadata can be inspected in the corresponding Maven POMs and source distributions. Bundled artifacts retain upstream notices.

Qwen and LiteRT LM are not bundled in Phase 1. Before Phase 4 distribution, include the selected artifact's full Apache 2.0 license and any NOTICE files, pin its revision/checksum, and add an in-app Open Source Licenses view covering the complete runtime dependency tree. Do not claim a model is installed before the weights are actually included and verified.
