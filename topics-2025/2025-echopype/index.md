---
title: Getting started with Echopype
---

Friday April 25 11am PT/2pm ET. This Friday's HackHour topic is Getting started with Echopype. In this session, you will get an introduction on using accessing echosounder data on the NOAA NCEI Water Column Sonar Data archive. Our guest speaker is [Wu-Jung Lee](https://uw-echospace.github.io/author/wu-jung-lee/) at the UW Applied Physics Lab.

## What is Echopype?
- An accidental package
- Stand on the shoulders of giants!
- **Compositional**: designed to be used with other packages
- Design philosophy: 
    - Scalable
    - Interoperable
    - Accessible
    - Reproducible
- Not for visual-based manual analysis
- The most mature package in the [Echostack](https://proceedings.scipy.org/articles/WXRH8633), many external users


## Some details
- [Echopype paper](https://doi.org/10.1093/icesjms/fsae133)
- Workflow
    - standardize and then compute
    ![image](https://echopype.readthedocs.io/en/latest/_images/workflow_v2.png)
- The `EchoData` object
    - gridded data: deviate from the SONAR-netCDF4 version 1 convention
    - some difference of variable names: not fully adapated to version 2 convention
    ![image](https://echopype.readthedocs.io/en/latest/_images/beam_dim_v5-01.png)
- [Development roadmap](https://echopype.readthedocs.io/en/latest/contrib_roadmap.html)
    - We need help!


## Demo notebooks

The two notebooks in the hackhour repo are copied from the [echopype-examples](https://github.com/OSOceanAcoustics/echopype-examples) repository, so they are "frozen" as of April 2025 and work with echopype v0.10.1. Go to the repo for the updated notebooks that would work with later echopype versions.

* [Getting started with Echopype](./getting_started.ipynb)
* [Watching a solar eclipse using a moored, upward-looking OOI echosounder](./OOI_eclipse.ipynb)


## Cloning the repo

The echopype tutorials are in `topics-2025/2025-echopype`

Never cloned the NMFSHackDays-2025 repo?

```
cd ~
git clone https://github.com/nmfs-opensci/NMFSHackDays-2025
```

Have cloned it but need to update? This is going to destroy any changes that you made to the repo to make it match the current state of the repo on GitHub.

```  
cd ~/NMFSHackDays-2025
git fetch origin
git reset --hard origin/main
```