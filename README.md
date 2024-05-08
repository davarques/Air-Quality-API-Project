# Air Quality Assessment for Business Locations
[![Alt text](https://www.epa.gov/sites/default/files/styles/medium/public/2021-05/aqaw_2021_0.png?itok=dMP6C0bR)](https://www.epa.gov/sites/default/files/styles/medium/public/2021-05/aqaw_2021_0.png?itok=dMP6C0bR)

## Context ♻️🏢

In today's business landscape, technological companies often outsource aspects of their workforce, such as sales, support, and operations, to external firms known as vendor partners to scale up operations.

Deciding where to open a new office or where to move your operations can include multiple key decisive factors into the equation like costs, connection, political stability, etc.

However, with the environment worsening, factors like air quality and pollution are definitely good decision-making points to take into account when opening new offices or business locations.

## Script / Usage 💻

This script allows you to analyze Air Quality data for different locations, aiding decisions about office locations. 

Here's what you can do:

1. **Analyze Air Quality**: Investigate the historic or current air quality of existing offices.
2. **Explore New Locations**: Input city details to assess air quality for potential new offices.
3. **Make Informed Decisions**: Utilize air quality insights to decide on office locations.
4. **Country Insights**: Obtain key country metrics such as Minimum Wage, Unemployment or Education rate. 
5. **Geographical Details**: Retrieve cities' longitude and latitude coordinates for air quality consultation.

## Project Overview 📋

In this study, we are assessing a specific scenario to simulate a study of deciding where to open a new office. The information we have for this case is:

**Where we are currently operating:**
- 🇮🇳 India: Gurugram, Hyderabad
- 🇵🇭 Philippines: Manila

### Problem Statement 🤔

- Investigate the current air quality of our operating locations.
- Explore potential new locations with similar costs and better air quality.

### Hypotheses 💭

#### Hypothesis 1:
The air quality in our current cities (Gurugram, Hyderabad, and Manila) is unhealthy or dangerous. Exploring new locations with better air quality is a good idea.

#### Hypothesis 2:
We can discover new locations to open offices that offer better air quality than our current sites (India and the Philippines) with similar labor costs, so we don't have to sacrifice much budget.

### Data Sources 💾 

| Data Source     | Link                                                  |
|-----------------|-------------------------------------------------------|
| **Air Quality API** | Source: [RapidAPI](https://rapidapi.com/weatherbit/api/air-quality/details)                                           |                                          |
| **Kaggle Datasets** | [World Cities Database](https://www.kaggle.com/datasets/max-mind/world-cities-database) |
|                  | [Global Country Information 2023](https://zenodo.org/records/8165229)    


## Findings and Insights 🎯

#### Hypothesis 1:

We reviewed the Air quality status of the current locations we operate and the results of Air Quality are:

![Screenshot 2024-04-20 at 14 23 50](https://github.com/davarques/Air-Quality-Analysis/assets/160759223/cdab1b94-7291-468b-8ecb-0439416f3c57)

---

#### Hypothesis 2:

1) First we assesed a sample of 141 countries, sorting Minimum wage & Unemployment from (Low to High) and Education 
(High to Low) to identify potential hotspots (in red) and this is the result:

![image](https://github.com/davarques/Air-Quality-Analysis/assets/160759223/9f7f0281-927a-467a-81d7-9c8347d54be3)

---

2) Secondly we reduced that sample focusing in the followinf filters:

- Minimum wage($) [0-2]
- Unemployment rate (%) [0-5]
- Gross primary education enrollment (%) > 110

  We identified a sample of 11 potential locations and created a Scatter Plot to visualize the data:

![Screenshot 2024-04-20 at 14 25 54](https://github.com/davarques/Air-Quality-Analysis/assets/160759223/61d58a9e-e04b-48c2-af68-b87f23657f9b)

---

3) Finally we ran the Air quality API for the four finalist locations and got the following results:

![Screenshot 2024-04-23 at 13 19 51](https://github.com/davarques/Air-Quality-Analysis/assets/160759223/f0a430bf-e02f-4960-aafa-7d2f9f5b0fc0)

## Conclusions 💡

- Two-thirds of our current locations are unhealthy 😷, and one-third is dangerous ☠️ in terms of Air Quality.
  
- If air quality is a crucial factor for our next location, exploring new places is worthwhile.
  
- Overall African countries 🌍 look like a good alternative 🔄 to explore, offering better air quality ♻️ while keeping costs 💰comparable to the Asian locations.
  
- Potenatial good candidates are: Guinea-Bissau, Madagascar and Togo, Madagascar ⭐ being the favourite for highest % education compared to ther other two. 

## Project Limitations ⚠️
- Air quality and labor costs (minimum wage, unemployment rate, and education) are not the only factors to consider when deciding new locations.
  
- This study is not definitive or final. Other factors, such as political stability, conflicts, or resources, could significantly influence the decision-making process when exploring new locations in Africa.
