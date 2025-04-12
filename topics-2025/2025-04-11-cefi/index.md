# CEFI Data access

Friday April 11 11am PT/2pm ET. This Friday's HackHour topic is Accessing CEFI data. In this session, you will get an introduction to accessing CEFI data via OPeNDAP, AWS and Google. Our guest speaker is ([Chia-Wei Hsu](https://github.com/chiaweh2), NOAA PSL).

# Building a Docker Image and Environment on 2i2c
To create a 2i2c-compatible Docker image for use with the notebook materials, please use the [CEFI Cookbook GitHub repository](https://github.com/NOAA-CEFI-Portal/cefi-cookbook). When setting up the environment, select the option to build the Docker image directly from the GitHub repository. Then add this repo url to the box
```
https://github.com/NOAA-CEFI-Portal/cefi-cookbook
```

<img width="855" alt="image" src="https://github.com/user-attachments/assets/9131f51b-624a-41c9-bd13-8173369f47c3" />

## Tutorials

* OPeNDAP - [python_get_cefi](https://nmfs-opensci.github.io/NMFSHackDays-2025/topics-2025/2025-04-11-cefi/python_get_cefi.html)
* Cloud - [python_get_cefi_cloud](https://nmfs-opensci.github.io/NMFSHackDays-2025/topics-2025/2025-04-11-cefi/python_get_cefi_cloud.html)
* OPeNDAP - [r_get_cefi](https://nmfs-opensci.github.io/NMFSHackDays-2025/topics-2025/2025-04-11-cefi/r_get_cefi.html) R in Jupyter Lab
* Cloud - [python_get_cefi_cloud](https://nmfs-opensci.github.io/NMFSHackDays-2025/topics-2025/2025-04-11-cefi/r_get_cefi_cloud.html) R in Jupyter Lab

## Some useful links

* [CEFI portal cookbooks](https://psl.noaa.gov/cefi_portal/#cookbooks)
* [CEFI portal](https://psl.noaa.gov/cefi_portal/#overview )
* [CEFI portal GitHub organization](https://github.com/NOAA-CEFI-Portal)
* [Data OPeNDAP](https://psl.noaa.gov/thredds/catalog/Projects/CEFI/regional_mom6/cefi_portal/catalog.html)

## Cloning the repo

Chia-Wei's tutorials are in `topics-2025/2025-04-11-cefi`

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