# **Introduction**
Airbnb functions as a marketplace linking property owners (hosts) with renters (guests). In recent years, Airbnb has transformed the hospitality industry globally, offering tourists and travelers a wide range of accommodations beyond traditional hotels. 
Every city has distinct criteria for popular Airbnb listings. Bangkok, a popular tourist destination with numerous Airbnb options. In this project we aim to understand the criteria of popular listings in Bangkok, Thailand.

# **Problem Statement**
What listing criteria do guests often choose when staying in Bangkok based on the number of reviews available? Considering the limited data we have, choosing the number of reviews is still appropriate to be able to find out what kind of listing criteria are often chosen by guests. Even though we don't know whether the guest likes it or not, we can ensure that the guest chooses the listing. 

The aim of this project is to explain the criteria of popular listings in Bangkok. These findings will enhance our understanding of the Airbnb market in Bangkok and provide valuable guidance for hosts and guests alike.

# **The Data**
- The data contains detailed information regarding Airbnb listings in Bangkok in 2022.
- There are 15,854 total entries.
- There are 16 attributes, and the following are the names and explanations of each attribute:
  - `name`
  - `host_name`
  - `neighborhood`
  - `room_type`
  - `prices`: Per day in local currency (baht)
  - `minimum_nights`
  - `number_of_reviews`
  - `last_review`: Date of most recent review
  - `reviews_per_month`

## **Data Cleaning**
In the data cleaning process we will handle missing values, duplicates, and outliers.

## **Adding New Columns**
To provide results that are easier to understand, we will create three new columns based on the existing columns:
- Area: Categorizes the neighborhood column into 4 categories.
  - CBD (Central Business District)
  - North Bangkok
  - West Bangkok
  - East Bangkok

- Stay Type: Categorizes minimum_nights into 3 categories.
  - Short Term: `minimum_nights` <= 7
  - Medium Term: `minimum_nights`<= 30
  - Long Term: `minimum_nights` > 30

- Price Type: Categorizes the price column into 3 categories based on the quartile value of the price column.
  - Economical: `price` <= 900 baht
  - Midrange: `price` <= 2429 baht
  - Luxurious: `price` > 2429 baht

# **The Analysis Summary**
To answer the main question, "What listing criteria do guests frequently choose when staying in Bangkok based on the number of reviews available?" we will divide it into several questions:
- Which area has the most total reviews?
- What type of room has the most total reviews?
- Which price type has the most total reviews?
By answering these questions, we can determine the key listing criteria that guests frequently choose when staying in Bangkok. This information will provide insights into guest preferences.

## **Most Popular Area**
![image](https://github.com/user-attachments/assets/829b220b-6282-4ea1-858e-e48214208b16)
- The CBD is the most popular area for guests, accounting for 75% of the total number of reviews.
- The CBD is the central financial and commercial area in Bangkok, showcasing luxurious metropolitan life.
- This indicates that guests prefer to stay in metropolitan areas, to start their Bangkok holiday.

## **Most Popular Room Type**
![image](https://github.com/user-attachments/assets/50e43563-c3f2-43a8-9d96-ac990b745413)
- The entire home/apt type of accommodation is the most popular with guests, accounting for 75% of reviews.
- This indicates that guests prefer to stay in a place that offer a home-like sensation, providing privacy and comfort.

![image](https://github.com/user-attachments/assets/1ca87b3a-d095-462b-a3c6-e4d902d12fe7)
- This indicates that guests prefer to stay in a place that offer a short duration of stay.

## **Most Popular Price Range**
![image](https://github.com/user-attachments/assets/cda53498-5b6c-4c27-863a-7c53ab6ffd8f)
- The midrange price type is the most popular with guests, accounting for 54% of reviews.
- This indicates that guests are willing to spend around 900–2,429 baht for comfortable room to stay.

# **Recommendation**
- The CBD area is the most in demand by guests. Hosts with listings outside the CBD can provide facilities that facilitate access to the CBD to attract more guests.
- Room types that provide privacy and comfort, such as entire home/apartment listings, are guests' favorites. Hosts should focus on offering aspects of privacy and comfort. Hotel and private room accommodations also have the potential to attract guests because these types conceptually provide privacy and comfort.
- Based on considerations of area, type of accommodation, and services, a price range of 900–2,429 baht is considered reasonable for guests staying in Bangkok.
- Hosts must ensure that guests leave reviews after their stay to receive valuable feedback.
