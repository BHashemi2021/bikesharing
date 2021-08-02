# Bikesharing
 NYC Citi Bike Sharing Program Examined 

## Background

 New York’s bike-share program, called Citi Bike, is to close the gap in providing services to the areas with the most needs. Docking stations and bikes will be available in Manhattan and in parts of Brooklyn, although plans are being developed to expand it further across Manhattan, Brooklyn and other part of the city. This study is to find out about the demographics of those who will be using the bikes, places of most need for the bikes. 

 Now that we've gotten a good idea of how to create our story, there is still some more work to be done to convince investors that a bike-sharing program in Des Moines is a solid business proposal. To solidify the proposal, one of the key stakeholders would like to see a bike trip analysis.


 ## Task

 We have been required to create two technical analysis deliverables and a written report to present our results. You will submit the following:

Deliverable 1: Changing Trip Duration to a Datetime Format
Deliverable 2: Creating Visualizations for the Trip Analysis
Deliverable 3: Creating a Story and Report for the Final Presentation



### Deliverable 1: Changing Trip Duration to a Datetime Format

Through the use of Pandas in the Jupyter Notebook and use of Python language the a DataFrame was created from the study file by the following code:


```ruby

df = pd.read_csv("resources/data/201908-citibike-tripdata.csv")

```

Then the Trip Duration variable column in the DataFrame was converted from an inter value to a DateTime variable by the following code in Jupyter Notebook:


```ruby
df['tripduration'] = pd.to_datetime(df['tripduration'], unit='s')

```

The resulting DataFrame is displayed in Figure 1.


#### Figure 1: The Trip Duration Column Converted to DateTime Variable

----------------------------
![trip-datetime-duration.png](https://github.com/BHashemi2021/bikesharing/blob/main/resources/images/trip-datetime-duration.png)

-----------------------------

## Deliverable 2: Creating Visualizations for the Trip Analysis


### A- Showing the amount of time bikes are checked out for all riders and genders (Figure 2).


#### Figure 2: The amount of time bikes are checked out by riders by all kinds of genders

----------------------------
![check-out-time.png](https://github.com/BHashemi2021/bikesharing/blob/main/resources/images/check-out-time.png)

-----------------------------


### B- How many trips are taken by the hour for each day of the week, for all riders and genders (Figure 3).

#### Figure 3: The number of trips taken by hour for each weekday by gender

----------------------------
![checkout-times-by-gender.png](https://github.com/BHashemi2021/bikesharing/blob/main/resources/images/checkout-times-by-gender.png)

-----------------------------


### C- A breakdown of what days of the week a user might be more likely to check out a bike, by type of user and gender.


#### Figure 4: Break down of days of a week bikes checked out by costumer type and gender
 
----------------------------
![user-trips-by gender-by weekday.png](https://github.com/BHashemi2021/bikesharing/blob/main/resources/images/user-trips-by%20gender-by%20weekday.png)

-----------------------------

### D- Trips by Weekday per Hour (Figure 5)

#### Figure 5: Trips by Weekday per Hour   
----------------------------
![trips-by-weekday-per-hour.png](https://github.com/BHashemi2021/bikesharing/blob/main/resources/images/trips-by-weekday-per-hour.png)

-----------------------------

### E- User Trips by Gender by Weekday (Figure 6)

#### Figure 6: User Trips by Gender by Weekday
----------------------------
![user-trips-by-gender-by-weekday.png](https://github.com/BHashemi2021/bikesharing/blob/main/resources/images/user-trips-by-gender-by-weekday.png)

-----------------------------



## Deliverable 3: Creating a Story and Report for the Final Presentation


### 1- The Tableau Story

The Tableau Story created about the bike trip is available at [this web address](https://public.tableau.com/app/profile/be.h1774/viz/NYCCitiBikeSharingAnalysis/DesMoinsBikeSharing#3) on Tableau website.



### The Software Used in this undertaking

`   * Jupyter Notebook
    * Python v.3.8.5 through Conda 4.10.1 
    * Tableau Desktop Public Edition
    * Tableau Web Edition
    * Pandas 
    
