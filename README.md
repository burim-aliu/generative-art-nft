# Generative NFT Art

## Introduction

The `generative-art-nft` repository is a library for creating generative art. It was developed for the purpose of creating NFT avatar & collectible projects.

## Features

### Generate over a million distinct images with less than 60 traits
The library allows you to generate images every distinct possible combination of your traits.

### Add rarity weights
The library also allows you to configure the image generation process in such a way that you have complete control over how rare each and every trait is.

### Generate compliant JSON metadata for your NFTs
There is now an added functionality to generate JSON metadata for your NFTs that are in compliance with OpenSea metadata requirements (and by extension, the general NFT metadata standard).

## Installation

**Clone this repository**

```git clone https://github.com/burim-aliu/generative-art-nft.git```

**Install required packages**

```pip install Pillow pandas progressbar2```  
```yarn add ipfs-car```  
```yarn add carbites-cli```  


Upload your input assets in the `assets` folder, fill up the `config.py` file, and then run `python nft.py`.  

In order to generate JSON metadata, define BASE_NAME, BASE_IMAGE_URL, and BASE_JSON in `metadata.py` and then run `python metadata.py`.  

In order to generate .car file for NFT.storage, run `yarn ipfs-car --pack <input directory> --output <output>`  

In order to split CARs, run `carbites split --size 100MB --strategy treewalk ***.car`  

In order to join CARs, run `carbites join <example-*.car> --output <example-joined.car>`  





