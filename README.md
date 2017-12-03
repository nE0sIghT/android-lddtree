android-lddtree
=======

Fork of lddtree.sh's fork by Natanael Copa

This is a shell version of pax-utils' lddtree for android binaries.
This tool is useful for resolving elf dependencies when building android
firmware.

This tool should be executed in android build environmend and depends on
binutils binaries - ```arm-linux-androideabi-objtree``` and
```arm-linux-androideabi-readelf```.
Prebuild binaries from ```prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9```
project may be used.

```
Usage: lddtree.sh [options] <-R root> ELFFILE...

Options:

  -a              Show all duplicated dependencies
  -x              Run with debugging
  -R <root>       Use this Android system tree
  --no-auto-root  Do not automatically prefix input ELFs with ROOT
  -l              Display output in a flat format
  -h              Show this help output
  -V              Show version information
```
