# Using Virtualizarr, Dask and Holoviz to explore NODD data

**Author:** [Rich Signell](https://opensciencecomputing.com/) (Open Science Computing)


We will use the notebook here to explore NODD data using holoviz, then create a virtual dataset using Virtualizarr, and then run an embarrassingly parallel job (construction of references for each file) using Dask, and then also use Dask for parallel data access in Xarray.  

[![Colab Badge](https://img.shields.io/badge/Open_in_Colab-blue?style=for-the-badge)][colab-link]
<a href="javascript:void(0);" onclick="openJupyterWidget('https://github.com/OpenScienceComputing/HackHours/blob/main/hackhours_demo.ipynb');">
    <img src="https://img.shields.io/badge/Open_in_JupyterHub-orange?style=for-the-badge" alt="JupyterHub Badge">
</a> [![Download Badge](https://img.shields.io/badge/Download-grey?style=for-the-badge)][download-link]

[download-link]: https://github.com/OpenScienceComputing/HackHours/blob/main/hackhours_demo.ipynb
[colab-link]: https://colab.research.google.com/github.com/OpenScienceComputing/HackHours/blob/main/hackhours_demo.ipynb
[jupyter-link]: https://nmfs-openscapes.2i2c.cloud/hub/user-redirect/lab?fromURL=https://raw.githubusercontent.com/OpenScienceComputing/HackHours/main/hackhours_demo.ipynb

Because the NMFS OpenScapes hub was not set up for dask at the time I developed the demo, I decided to use Coiled for Dask.

To allow folks to try Coiled, but without signing up, you can use a token I created that expires in one day. To use the token to run COILED, login to the [NMFS OpenSpaces 2i2c JuptyerHub](https://nmfs-openscapes.2i2c.cloud/) with the default environment, open a terminal and type:
```
coiled login --token af791b1a879e4c0b99a8b7bec850e9a1-1e7144a190114be06abf273052d98640b62cb5fa
```

I created the named coiled environment by creating a [conda environment file](hackhours_coiled_env.yml) that matched the package versions in the JupyterHub default environment, as of 2025-03-21, via this command:

```
coiled env create --name hackhours-arm --workspace esip-lab --conda hackhours_coiled_env.yml --architecture aarch64
```


## How to download and open the tutorials

### Jupyter Hub

1. Start the Jupyter Hub server <nmfs-openscapes.2i2c.cloud>
2. Click the orange Open in Jupyter Hub button

### Colab

1. Click the Open in Colab button

### Download 

1. Download to your local computer
2. You will need to have Python and Jupyter Lab installed
3. Install any needed packages

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



