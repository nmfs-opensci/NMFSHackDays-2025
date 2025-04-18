# Working with Google Cloud Storage (GCS)

Friday April 18 11am PT/2pm ET. This Friday's HackHour topic is Accessing CEFI data. In this session, you will get an introduction to accessing CEFI data via OPeNDAP, AWS and Google. Our guest speaker is ([Chia-Wei Hsu](https://github.com/chiaweh2), NOAA PSL).

## Tutorials

I will be showing how I created this [NOAA WR17+18 Daily Mean Streamflow Dataset](https://noaa-nwfsc.github.io/Streamflow-Means-NWM/) and uploaded to Google Cloud Storage in our NODD.

## Some useful links

* [NOAA Open Data Dissemination Program Datasets](https://www.noaa.gov/nodd/datasets)
* [NMFS Google Cloud Storage](https://www.noaa.gov/nodd/datasets#NMFS)

## Cloning the repos

### Streamflow

```
cd ~
git clone https://github.com/noaa-nwfsc/Streamflow-Means-NWM
```

###  NMFSHackDays-2025

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