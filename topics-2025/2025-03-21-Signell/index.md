# Using Virtualizarr, Dask and Holoviz to explore NODD data

**Author:** [Rich Signell](https://opensciencecomputing.com/) (Open Science Computing)


We will use the notebook here to explore NODD data using holoviz, then create a virtual dataset using Virtualizarr, and then run an embarrassingly parallel job (construction of references for each file) using Dask, and then also use Dask for parallel data access in Xarray.  

Because the NMFS OpenScapes hub was not set up for dask at the time I developed the demo, I decided to use Coiled for Dask.

To allow folks to try Coiled, but without signing up, you can use a token I created that expires in one day. To use the token to run COILED, login to the [NMFS OpenSpaces 2i2c JuptyerHub](https://nmfs-openscapes.2i2c.cloud/) with the default environment, open a terminal and type:
```
coiled login --token af791b1a879e4c0b99a8b7bec850e9a1-1e7144a190114be06abf273052d98640b62cb5fa
```

I created the named coiled environment by creating a [conda environment file](hackhours_coiled_env.yml) that matched the package versions in the JupyterHub default environment, as of 2025-03-21, via this command:

```
coiled env create --name hackhours-arm --workspace esip-lab --conda hackhours_coiled_env.yml --architecture aarch64
```




