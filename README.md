# French Housing Price Estimation

This project tackles the regression task of estimating French housing real estate prices, a complex and widely studied problem. The dataset includes both **hierarchical tabular data** and **photos of real estate assets**, allowing for an exploration of whether the addition of visual information improves prediction accuracy.  

**Key Achievement:** Achieved a **Mean Absolute Percentage Error (MAPE)** score of **29.7**, without using the photos in the dataset.  

## Project Description

Estimating real estate prices is a common problem in real estate analytics, with an extensive literature focusing on using structured data such as:
- Location (latitude, longitude, postal code, city, etc.)
- Property characteristics (size, land area, number of rooms, etc.)
- Building specifics (age, energy performance indicators, etc.)

While these approaches generally yield adequate price range estimations, they often lack precision. This project explores whether incorporating **photos of the asset** (1 to 6 per listing) could enhance price estimation accuracy by providing complementary information.  

In this repository, we focus on:
1. **Modeling housing prices** using tabular data.
2. **Investigating interpretability** to identify the most valuable features.
3. **Laying the foundation for integrating visual data**, though the photos were not used in the current implementation.  

## Data Description

### Output
- **Target variable (`y`)**: Offered housing real estate prices in euros.

### Input Features (`X`)
1. **Listing Identifier**: Unique identifier for each listing.
2. **Property Characteristics**:  
   - Property type (house, apartment, mansion, etc.)
   - Location: Latitude, longitude, city, postal code, floor (if applicable), etc.
   - Size: Living area, land area (if applicable).
   - Number of rooms, bedrooms, bathrooms, etc.
   - Energy performance indicators (energy consumption and greenhouse gas emissions).
3. **Additional Features**:  
   - Presence of cellar, balcony, air conditioning, etc.
   - Number of photos attached to the listing.
4. **Photos**: A folder named `ann_XX` contains 1 to 6 photos for each listing, where `XX` corresponds to the listing identifier.  

The dataset offers a rich combination of structured data and visual elements to assess the impact of photos on model performance.


## Objectives
1. Build a robust regression model for housing price estimation.
2. Analyze feature importance and interpret model predictions to identify key drivers of price variability.
3. Lay the groundwork for integrating visual data into the modeling pipeline to improve prediction precision.  

## Results Interpretability
To enhance understanding of the price estimation process, we value interpretability by investigating:
- Feature importance rankings.
- Relationships between key variables and price predictions.  

## Next Steps
1. **Incorporate Photos**: Experiment with multimodal models that combine tabular data and images.
2. **Fine-tune Models**: Explore advanced architectures and hyperparameter optimization to further reduce the MAPE score.


