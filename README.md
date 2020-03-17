# Berlin House Rental Market Analysis

## Introduction

This project consists of an analysis of the some listings found online pertaining to the Berlin house rental market. 
While going through the process of finding a house to rent in Berlin, for some months I collected data on 
the market from the website immobilienscout24 for certain areas of Berlin.

With the data I collected, I was interested in answering some questions to help me in my search, including:

- What are the most and less expensive areas?
- What is the most popular time to publish a new listing?
- Am I paying a fair price?
- What makes some listings more attractive than others?

The analysis executed step by step can be found in the notebook `berlin-houses.ipynb`.

The main takeways are:

- the most expensive surveyed neighbourhood was Mitte, and the least one was Wedding. 
- the most popular time for publishing new listings was in the morning.
- the most important predictors for the warm price were if a listing is not located in the neighbourhoods of Wedding 
or Schöneberg, and if it has a built-in kitchen or a garden.
- the characteristics that are mostly associated with more interest in a listing are if it is new, 
has a built-in kitchen or a balcony as well as having more rooms and living space. As for the most sought after areas, 
it was observed that the most attractive neighbourhoods were Schöneberg, Tiergarten, Mitte, Treptow and Kreuzberg.

## Installation

In order to create a virtual environment for the project using conda, run the following command a the root of the project:

```conda env create --file environment.yaml```

Alternatively you can create a virtual environment with the provided `requirements.txt`

## Libraries used

The main libraries used (along with their respective dependencies) are:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## Dataset

The dataset used for the analysis can be found in the file `berlin-houses.csv`

The variables of this dataset are:

- `id` - id of listing
- `lat` - latitude of the listing
- `lon` - longitude of the listing
- `cold_price` - price of the listing before heating and upkeep costs
- `warm_price` - price of the listing after heating and upkeep costs
- `currency` - currency of the listing prices
- `short_listed` - if a given listing has short listed candidates
- `postcode_id` - post code of the listing
- `balcony` - if a listing has a balcony
- `builtin_kitchen` - if a listing has a built-in kitchen
- `created_date` - date the listing was created
- `modified_date` - date the listing was modified
- `published_date` - date the listing was published
- `energy_certificate` - if a listing has an energy certificate
- `has_new_flag` - if a listing is a new build or has been renovated recently.
- `living_space` - the living area in squared meters (m2)
- `new_home_builder` - if a listing has been built by new building company
- `number_rooms` - total number of rooms in listing
- `private_offer` - if a listing is pusblished by private owner
- `address` - address of the listing
- `link` - link to listing page
- `quarter` - district where listing is located
- `garden` - if a listing has a garden
- `listing_type` - listing size category
- `localhost_date` - date when listing data was saved into database
- `no_longer_available` - if listing is no longer available in website
- `no_longer_available_date` - date when listing was no longer available on the website