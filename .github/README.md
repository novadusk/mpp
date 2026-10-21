# Rockchip Media Process Platform

**Hardware video processing through Rockchip's MPP interfaces.** Explore the public API, buffer and frame objects, codec implementations and hardware abstraction layer.

[Public API](../inc/) · [Encode/decode tests](../test/) · [Design documents](../doc/) · [Original README](../readme.txt)

> novadusk fork of [rockchip-linux/mpp](https://github.com/rockchip-linux/mpp), on branch `develop`. Upstream platform and codec support are documented in the original README.

## Follow the data path

`Application / MPI → MPP buffer, frame and packet objects → codec / HAL → device`

| Path | Role |
| --- | --- |
| [inc/](../inc/) | Public interfaces and types |
| [mpp/](../mpp/) | Framework, codec processing and HAL implementations |
| [osal/](../osal/) | Operating-system abstraction |
| [test/](../test/) · [utils/](../utils/) | Test applications and supporting utilities |
| [build/](../build/) · [CMakeLists.txt](../CMakeLists.txt) | Build scripts and CMake configuration |

## Build and integration

Start with the target-specific scripts in [build/](../build/) and the [original build notes](../readme.txt). MPP uses CMake out-of-source builds. Select dependencies and libraries for the actual Rockchip target; upstream no longer maintains Windows support.

The original [readme.txt](../readme.txt) remains unchanged and contains detailed directory, platform and integration information. See [LICENSES/](../LICENSES/) and source-file notices for licensing.
