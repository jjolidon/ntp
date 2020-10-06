# About this repository

This is a fork of the original NTP code found at github.com/ntp-project/ntp .
The following changes have been made to support features of interest on Windows:

- Addition of Visual Studio 2017 and 2019 targets
- Activation of the shared memory reference clock that was disabled in the upstream repository
- Addition of ACL for the shared memory segment based on a registry key.

Due to the unreliable publication schedule of the upstream repository, I have switched to a dump-and-commit model for the repository:

- The upstream branches contain the codebase from NTP as can be downloaded from ntp.org
- The sharedmem branches contain the modified codebase for each implemented version
- The sharedmem commits are cherry-picked into the newer version, making changes as needed

I plan to make this repository read-only at a future point, as soon as I can drop dependency on the obsolete ntp codebase and switch to a more modern implementation.

I make no claim about the suitability of the code found in this repository. 
The software is provided as-is by its original authors without express or implied warranty.
The software remains the property of its original authors.

The modifications I made in the software are provided as-is without express or implied warranty.
The modifications I made to the software can be freely redistributed under the MIT license.
