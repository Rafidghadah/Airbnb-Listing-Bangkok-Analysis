# **Introduction**

# **Problem Statement**
What listing criteria do guests often choose when staying in Bangkok based on the number of reviews available? Considering the limited data we have, choosing the number of reviews is still appropriate to be able to find out what kind of listing criteria are often chosen by guests. Even though we don't know whether the guest likes the accommodation or not, we can ensure that the guest chooses the accommodation.

# **The Data**
- The data contains detailed information regarding Airbnb listings in Bangkok in 2022.
- The data was obtained from the Kaggle site.
- There are 15,854 total entries.
- There are 16 attributes, and the following are the names and explanations of each attribute:
  - name
  - host_name
  - neighborhood
  - room_type
  - prices: Per day in local currency (baht)
  - minimum_nights
  - number_of_reviews
  - last_review: Date of most recent review
  - reviews_per_month

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
  - Short Term: minimum_nights <= 7
  - Medium Term: `minimum_nights`<= 30
  - Long Term: minimum_nights > 30

- Price Type: Categorizes the price column into 3 categories based on the quartile value of the price column.
  - Economical: price <= 900 baht
  - Midrange: price <= 2429 baht
  - Luxurious: price > 2429 baht

# **The Analysis**


# **Recommendation**









# **Latar Belakang**
Airbnb adalah sebuah marketplace online yang menghubungkan orang-orang yang ingin menyewa atau menyewakan propertinya, seperti kamar pribadi, apartemen, villa, atau rumah. Airbnb didirikan pada tahun 2008 di San Francisco, California, Amerika Serikat. Sebagai salah satu platform online terbesar di dunia, analisis data dari jutaan penginapan di platform ini menbjadi faktor penting bagi perusahaan. Hasil analisis data ini dapat digunakan untuk berbagai tujuan, seperti pengambilan keputusan bisnis, pemasaran, dan inovasi layanan.

Departement *Host and Guest Services* di Airbnb bertanggung jawab untuk memastikan pengalaman positif bagi *host* dan *guest*. Salah satu tantangan yang mereka hadapi adalah mengidentifikasi kriteria yang mempengaruhi *guest* untuk memilih listing di Bangkok. 

Kriteria tersebut akan digunakan Departement *Host and Guest Services* sebagai materi pendukung dalam merumuskan panduan bermanfaat yang dapat digunakan para *host* untuk meningkatkan performa listing mereka.

# **Pernyataan Masalah**
Apa saja kriteria yang mempengaruhi *guest* untuk memilih listing di Bangkok? dan bagaimana Departement *Host and Guest Services* dapat menggunakan hasil analisis ini untuk membantu *host* untuk meningkatkan performa listing mereka?
