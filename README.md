# spinalcordtoolbox-binaries
Binary packages for the C++ dependencies of [neuropoly/spinalcordtoolbox](https://github.com/neuropoly/spinalcordtoolbox)

This is essentially a metapackage of three packages:

- [ANTS](https://github.com/ANTsX/ANTs) (but only a portion of it; the whole thing is too large)
- some [custom tools](https://github.com/neuropoly/spinalcordtoolbox/blob/master/dev) for research and development
- [ctrDetect](https://www.creatis.insa-lyon.fr/site7/en/ctrDetect)

Unlike a traditional metapackage, instead of including links to the contained packages this directly copies them into it. We distribute them together because it simplifies our package manager, `sct_download_data`, to only have to track and know about one big file.

See [.github/workflows/package-binaries.yml](.github/workflows/package-binaries.yml) for the packaging script, and the links to update to change the included versions.
