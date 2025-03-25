---
title: Intro to Dask
---

In this session, you will get an introduction to [Dask](https://www.dask.org/) for parallel computing in Python.  You learn about local Dask clusters to run tasks on all your CPUs versus Dask Gateway and Coiled clusters. The nmfs-openscapes Jupyter Hub is set-up with Dask Gateway to allow Gateway; it is a common but not a default feature of Jupyter Hubs. Coiled will require a Coiled account and your own AWS, GCP, Azure or other cloud account where your new pods (virtual machines) will be spun up.

When you start up the Jupyter Hub, please select the "Py - NASA Openscapes Python 07980b9" image not the default image. This is smaller and the Gateway pods will start faster.

| Feature                 | `LocalCluster`  | `DaskGateway`   | `Coiled` |
|------------------------|----------------|---------------|---------------|
| Runs in your Jupyter Hub cloud   ? | ✅ Yes      | ✅ Yes  (in new pods in the hub)   | ❌ No (runs in new pods on AWS, GCP, Azure, or others)       |
| Runs in your notebook? | ✅ Yes      | ❌ No (runs in new pods)    | ❌ No (runs in new pods)       |
| Uses multiple pods?    | ❌ No       | ✅ Yes (scheduler + workers)   |  ✅ Yes 
| Scales beyond pod?     | ❌ No       | ✅ Yes                         |  ✅ Yes 
| Can use files in /home |  ✅ Yes     | ❌ No                          |  ❌ No 

## Tutorials

* [Local clusters](https://nmfs-opensci.github.io/NMFSHackDays-2025/topics-2025/2025-dask/Dask_local_cluster.html)
* [Gateway clusters](https://nmfs-opensci.github.io/NMFSHackDays-2025/topics-2025/2025-dask/Dask_gateway.html)
* [Coiled clusters](https://nmfs-opensci.github.io/NMFSHackDays-2025/topics-2025/2025-dask/Dask_coiled.html)

## How to download and open the tutorials

### Jupyter Hub

1. Start the Jupyter Hub server <nmfs-openscapes.2i2c.cloud>
2. Click the orange Open in Jupyter Hub button

### Colab

1. Click the Open in Colab button. You will need to install  dask, dask-labextension, dask-geopandas, coiled. Gateway will not work as that is for a hub on top of Kubernetes.

### Download 

1. Download to your local computer. Dask works on local computers or standalone virtual machines.
2. You will need to have Python and Jupyter Lab installed
3. Install any needed packages. You will need to install  dask, dask-labextension, dask-geopandas, coiled. Gateway will not work as that is for a hub on top of Kubernetes.

### How to clone the git repository

After cloning, you will need to navigate to the tutorials in the `topics-2025` directory.

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
