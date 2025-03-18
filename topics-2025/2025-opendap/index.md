---
title: OPeNDAP - Python
---

In this session, you will get an introduction to accessing data on data servers that provide [OPeNDAP](https://www.opendap.org/) for data access. [What is OPeNDAP](https://www.opendap.org/about/what-is-opendap/)? "OPeNDAP is the commonly used name for a discipline-neutral data access protocol (DAP) that’s widely utilized both to access and to provide data over the internet. You will find lots of data servers that use OPeNDAP.

Note, these tutorials are narrowly focused on an `xarray` workflow with `earthaccess` handling authentication and `pydap` as the underlying engine. 
The goal is to create a lazy (no data loaded) `xarray` data cubes via `open_dataset` and `open_mfdataset` functions.

If you use NASA data, they are migrating to serving their data to the cloud and you should look at the `earthaccess` examples for data access. If you use NOAA data, they use a lot of ERDDAP servers, which are built off OPeNDAP but have some extra features. Go to the ERDDAP examples. If your data are somewhere in a cloud-native format (Zarr, geotiff) use that. That is going to be a lot easier (and faster) to work with for the xarray workflows that I focus in the 2025 HackDays tutorials. 

## Tutorials

* Simple example 1 with no authentication needed. [NCEP-NCAR](1-ncep-ncar.html)
* Simple example 2 with no authentication needed. [Delaware Bay Operational Forecast System ](2-dbofs.html)
* NASA OPeNDAP servers, authentication needed. [NASA OPeNDAP](3-earthdata-auth.html)
* NSIDC server, NASA Earthdata authentication needed. 
* USDA LPDAAC server, NASA Earthdata authentication needed. 

## Servers that use NASA Earthdata authentication

Things with `nasa.gov` are obvious but a couple others without nasa.gov in the url also use it.

* list (not fully up to date) of NASA opendap servers: <https://www.earthdata.nasa.gov/engage/open-data-services-software/earthdata-developer-portal/opendap/servers>
* NSIDC <https://n5eil02u.ecs.nsidc.org/opendap/> [docs](https://nsidc.org/data/user-resources/help-center/how-do-i-access-data-using-opendap) 
* USGS LPDAAC <https://opendap.cr.usgs.gov/opendap/hyrax/>

## References

* [xarray support for opendap](https://docs.xarray.dev/en/stable/user-guide/io.html#opendap)
* [pydap](https://pydap.github.io/pydap/intro.html)
* <https://github.com/ornldaac/daymet-python-opendap-xarray>
* <https://github.com/podaac/tutorials/blob/master/notebooks/opendap/MUR-OPeNDAP.ipynb>
* <https://earthaccess.readthedocs.io/en/latest/user-reference/api/api/#earthaccess.api.get_requests_https_session>
* <https://podaac.jpl.nasa.gov/OPeNDAP-in-the-Cloud>
