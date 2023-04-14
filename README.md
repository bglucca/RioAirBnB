# RioAirBnb

## Motivation

For this project I wanted to make initial explorations into ways to facilitate searching through listings in AirBnb for the city of Rio de Janeiro, Brazil.  
Rio was chosen since it's my hometown and therefore I would be able to shed some context into the data, if needed.

### Main Questions

With this motivation in mind the analysis was centered in four questions regarding different aspects of the dataset:

- Where are the cheapest options located? (Where to look for)
- Can we pre-segment listings by their characteristics? (Be able to see specific Groups of listings)
- Are the location prices and cluster prices associated to market concentration? (Avoid skewed prices)
- What are usual amenities that the customer should expect from listings in Rio? (Set expectations)

## Result Summary

*Where are the cheapest options located?*  
**On the North and Central regions of the city. We can also get results for the 5 cheapest neighbourhoods within each region**  

*Can we pre-segment listings by their characteristics?*  
**Yes. We can find 8 clusters that arise from the variables that describe a listing using a KModes algorithm**

*Are the location prices and cluster prices associated to market concentration?*  
**No evidence in the available data was found that indicates that prices are skewed due to concentration, either looking at it geographically, within the clusters or at the whole dataset in general**

*What are usual amenities that the customer should expect from listings in Rio?*  
**A customer should expect: Wifi, a Kitchen, Long term stays permission, Essentials, Hangers, Iron, Hot water, Dishes and silverware, Air conditioning, Elevator as the top-10 most frequent amenities.**  
**On the other hand, they should expect: Beachfront properties, Private patio or balcony, Gym, Dryer, Window AC unit, Portable fans, Free washer In unit, Security cameras on property, Toasters and BBQ grill as more rare amenities**

## Libraries

- **Data Wrangling**: Pandas, Numpy
- **Data Viz**: matplotlib, seaborn
- **Text Wrangling**: re, unidecode
- **Data Modelling**: [KModes](https://pypi.org/project/kmodes/)

## Repo Structure

```
│   analysis.ipynb -> Main notebook containing all analysis and modelling  
│
├───data
│       listings.csv.gz -> listing data used  
│
├───models
│       clusters.pkl -> A pickle with the final clustering model
```

## Acknowledgements
Data sourced from [Inside AirBnb](http://insideairbnb.com/get-the-data/)  
KModes supporting papers' links along with the implementation used can be found in [nicodv's GitHub repo](https://github.com/nicodv/kmodes)  
This project was is a submission for Udacity's Nanodegree Programm for Data Science  
The article for this project can be found on my [Medium Page](https://medium.com/@luccagomes/making-browsing-airbnb-easier-through-data-science-bf96e2a72e0c)
