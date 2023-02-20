# SSE-Ghidra-Tutorial

## Tutorial

### Install Ghidra

Ghidra is an open-source java software retro-engineering suite of tools.
It will work on Windows, Linux, MacOS.   
https://ghidra-sre.org/

### Steamless skyrim.exe

You need to steamless the skyrim executable to be able to retro-engineer it efficiently.   
Here is the software:
https://github.com/atom0s/Steamless/releases

Then apply it on your skyrim executable, produce the steamlessed version and save it.
We will work on this one. 

In this version of the tutorial, we'll focus on using the 1.5.97 version of the skyrim executable.

## Notes

- Use a 1.5.97 build as base.
- Version track to other versions (1.6.640, 1.6.353, VR)
- Import the pdbs posted with Crashlogger to get the latest labels including what -- posted, into Ghidra. That will give names.
- There's a types.h floating on the the re server with 1.5.97 data structures from like 3 years ago to get started.
- We really need some tooling to just convert commonlib to something importable for types
- With Ghidra, first import pdb, then perform auto analysis for each exe.
- After done, do version tracking and do auto version analysis. That may take a few days to process though.
- It's possible the pdb includes the types but I haven't checked. Just recently figured out exporting pdbs from Ghidra.
