##  Predicting uranium deposits size by observed indicators

### Problem

1) the "on ground" researches are very expensive and time-consuming

### Solution

1) we will create tool for uranium deposit size prediction bsed on observed
indicators

### Dataset

At first stage we define list of domains, from where we can receive the data

1) soil composition [link](https://www.fao.org/soils-portal/data-hub/soil-maps-and-databases/harmonized-world-soil-database-v12/en/)
2) height of the surface [link](http://maps.google.com)
3) earthquaqes [link](https://public.opendatasoft.com/explore/dataset/significant-earthquake-database/table/?location=8,41.81636,46.7688&basemap=jawg.light)
1) Uranium deposits australia only png [link](https://www.ga.gov.au/digital-publication/aecr2021/uranium-and-thorium)
1) Thorium depositsaustralia only png [link](https://www.ga.gov.au/digital-publication/aecr2021/uranium-and-thorium)
1) historical weather api [link](https://open-meteo.com/en/docs/historical-weather-api#location_mode=csv_coordinates&timezone=Asia%2FBangkok)
2) Uranium deposits usa [link1](https://www.arcgis.com/home/item.html?id=1ddc80916bb742cfb439fef2cfe56b8d), [link2](https://www.sciencebase.gov/catalog/item/5d1ce678e4b0941bde64cd71)
3) canada no areas [link](https://world-nuclear.org/information-library/country-profiles/countries-a-f/canada-uranium.aspx), only mines no areas [link](https://open.canada.ca/data/en/dataset/ce375e21-8893-11e0-8e6c-6cf049291510)

### Problems

With each source of data there are a lot of problems, which in general don't allow to
create dataset with proper quality

#### Soil composition 

The first source was the [Harmonized soil database](https://www.fao.org/soils-portal/data-hub/soil-maps-and-databases/harmonized-world-soil-database-v12/en/).
The map contains good level of global detalization, but there are a lot of problems 
in small regions. For example, for Armenia there are only 4 types of soils, but in reality there are 
more types

<img src="images/soil_types.jpg" width="300" />

If we use the typical soil composition maps, we will see that there is no unification. There are soil types, that
Armenia has and Australia doesn't and vice versa. 

![biba](images/soil_type_arm.png)

<img src="images/soil_type_au.jpg" width="300" />

Also it is unclear how to transfer the soil maps from png to discrete system. 

#### Height of the surface



### Results

Research shows, that it is very difficult and sometimes almost impossible 
to create dataset based on quasi-opened data. 
The is no county in the world that openly distributes the strategic resources data.
Furthemore, it's not clearn how to transfer data from resources maps to discrete grid
without big losses

The data sources, where there were no problems, are map of earthqueaqes and height map

