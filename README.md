# Project Description
In this project, exploratory data analysis is performed on hotel bookings' data using **Python**, with relevant elaborations and visualisations presented together using **Jupyter Notebook**. There are a few key focuses for this project:
* To investigate factors impacting **cancellation rates** at hotels
* To investigate **[ADR](https://www.investopedia.com/terms/a/average-daily-rate.asp) (average daily rate) relationships** with other categories of hotel data
* To identify opportunities for hotels to **maximise revenue**

The project involves the following steps:

* **Data Sourcing and Uploading**: A suitably large, free-to-use dataset containing multiple factors is located and downloaded.
* **Data Cleaning and Initial Exploration**: The dataset is cleaned such as through deletion of null values, and initial details involving datatypes and statistics are obtained.
* **Exploratory Data Analysis**: Additional features (i.e. categories) are engineered involving use of user-built function, and various code segments are written to draw valuable insights mainly in the form of visualisations.

# Dataset Details
The dataset used in this project is from Kaggle and is derived from an actual case study involving two hotels, with individually identifiable details having been omitted. The dataset contains details pertaining to hotel booking and cancellation data, including countries, arrival dates, and lead time. Additional details as well as the raw dataset can be found [here](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/).

# Summary of Insights
Having concluded the exploratory data analysis, we can summarise key insights drawn and focus areas from two different angles as follows:

**Cancellations**:

1. The city hotel has both a higher count of cancellations as well as a higher cancellation percentage (~41.7% vs 28.0%), making it important to focus on.
2. Cancellation percentages are fairly constant throughout the year, with the monthly count data appearing to resemble that of a normally distributed dataset. This, however is likely to be coincidental due to increased travel preferences during the European summer period (i.e. July, August)
3. Portugal is solely responsible for 27,514 cancellations, which is ~23.1% of all bookings. There is a huge opportunity to reduce cancellations by delving deeper into this observation. It should also be noted that looking at the top 10 countries, bookings are mostly from the European and Great Britain countries.
4. A higher lead time is clearly linked to cancellations, with a lead time of ~20-30 days representing the period with the highest data density and therefore a possible focus area.
5. The engineered feature of non-matching rooms (looking at reserved vs assigned rooms) interestingly does not show any impact on cancellations, with almost all non-matching rooms falling under non-cancelled bookings.

**ADR (Average Daily Rate)**:

1. The mean ADR shows an increasing monthly trend until August before decreasing, while cancellation percentages remain fairly constant throughout the year. This implies good maximisation of revenue from the hotels without impacting cancellation percentages.
2. A clear cyclical trend can be observed looking at the mean ADR trend for the resort hotel, with months in the European summer season heavily favoured over the other months in a year. Also noteworthy are the spikes in ADR during New Year’s Day for the resort hotel, again demonstrating good capitalisation of inelastic demand during that period.
3. There exists some room to explore matching the ADR of non-transient customer types (~75-85) to the main transient customer type at 90-95, to increase overall revenue.
