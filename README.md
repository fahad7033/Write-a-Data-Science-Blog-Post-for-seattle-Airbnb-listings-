# Data Science Blog Post for seattle Airbnb listings dataset

AS a part of the Udacity data scientist nanodegree, this blog post presents 3 business questions about Seattle Airbnb Dataset. The reference of the dataset is presented at the end of the post.
The dataset contains the listing details of homestays inSeatle. 3818 listings details are available in the dataset (92 features) as shown below:

RangeIndex: 3818 entries, 0 to 3817
Data columns (total 92 columns):
id                                  3818 non-null int64
listing_url                         3818 non-null object
scrape_id                           3818 non-null int64
last_scraped                        3818 non-null object
name                                3818 non-null object
summary                             3641 non-null object
space                               3249 non-null object
description                         3818 non-null object
experiences_offered                 3818 non-null object
neighborhood_overview               2786 non-null object
notes                               2212 non-null object
transit                             2884 non-null object
thumbnail_url                       3498 non-null object
medium_url                          3498 non-null object
picture_url                         3818 non-null object
xl_picture_url                      3498 non-null object
host_id                             3818 non-null int64
host_url                            3818 non-null object
host_name                           3816 non-null object
host_since                          3816 non-null object
host_location                       3810 non-null object
host_about                          2959 non-null object
host_response_time                  3295 non-null object
host_response_rate                  3295 non-null object
host_acceptance_rate                3045 non-null object
host_is_superhost                   3816 non-null object
host_thumbnail_url                  3816 non-null object
host_picture_url                    3816 non-null object
host_neighbourhood                  3518 non-null object
host_listings_count                 3816 non-null float64
host_total_listings_count           3816 non-null float64
host_verifications                  3818 non-null object
host_has_profile_pic                3816 non-null object
host_identity_verified              3816 non-null object
street                              3818 non-null object
neighbourhood                       3402 non-null object
neighbourhood_cleansed              3818 non-null object
neighbourhood_group_cleansed        3818 non-null object
city                                3818 non-null object
state                               3818 non-null object
zipcode                             3811 non-null object
market                              3818 non-null object
smart_location                      3818 non-null object
country_code                        3818 non-null object
country                             3818 non-null object
latitude                            3818 non-null float64
longitude                           3818 non-null float64
is_location_exact                   3818 non-null object
property_type                       3817 non-null object
room_type                           3818 non-null object
accommodates                        3818 non-null int64
bathrooms                           3802 non-null float64
bedrooms                            3812 non-null float64
beds                                3817 non-null float64
bed_type                            3818 non-null object
amenities                           3818 non-null object
square_feet                         97 non-null float64
price                               3818 non-null object
weekly_price                        2009 non-null object
monthly_price                       1517 non-null object
security_deposit                    1866 non-null object
cleaning_fee                        2788 non-null object
guests_included                     3818 non-null int64
extra_people                        3818 non-null object
minimum_nights                      3818 non-null int64
maximum_nights                      3818 non-null int64
calendar_updated                    3818 non-null object
has_availability                    3818 non-null object
availability_30                     3818 non-null int64
availability_60                     3818 non-null int64
availability_90                     3818 non-null int64
availability_365                    3818 non-null int64
calendar_last_scraped               3818 non-null object
number_of_reviews                   3818 non-null int64
first_review                        3191 non-null object
last_review                         3191 non-null object
review_scores_rating                3171 non-null float64
review_scores_accuracy              3160 non-null float64
review_scores_cleanliness           3165 non-null float64
review_scores_checkin               3160 non-null float64
review_scores_communication         3167 non-null float64
review_scores_location              3163 non-null float64
review_scores_value                 3162 non-null float64
requires_license                    3818 non-null object
license                             0 non-null float64
jurisdiction_names                  3818 non-null object
instant_bookable                    3818 non-null object
cancellation_policy                 3818 non-null object
require_guest_profile_picture       3818 non-null object
require_guest_phone_verification    3818 non-null object
calculated_host_listings_count      3818 non-null int64
reviews_per_month                   3191 non-null float64
dtypes: float64(17), int64(13), object(62)
memory usage: 2.7+ MB


Here, there are 3 business questions asked that we are trying to answer:
•	Which type of properties has the highest number of hosts? 
•	What are the top 5 neighborhoods that have the maximum number of hosts?
•	Which neighborhoods have the highest average of prices and the neighborhoods have the lowest average of prices?

# Question 1: Which type of properties has the highest number of hosts? 
In the listing dataset there are 16 types of properties. The types of properties that have the maximum number of hosts are houses and apartments. Houses represent 45.75% of the listings where apartments represent 44.46% of the listings. The below chart shows the count of properties according to each type.  
 


# Question 2: What are the top 5 neighborhoods that have the maximum number of hosts?
The hosts in the listings are offered within 81 neighborhoods. However, there are some neighborhoods have more number of hosts. The data shows that 10.32% of the hosts are located in “Capitol Hill”. Here are the top 5 neighborhoods that have the maximum number of hosts:
•	Capitol Hill    10.320494
•	Ballard          6.262864
•	Belltown         5.998236
•	Minor            5.645398
•	Queen Anne       5.498383
The chart below shows the number of hosts for every neighborhood:






# Question 3: Which neighborhoods have the highest average of prices and the neighborhoods have the lowest average of prices?
According to the data, “Fairmount Park” has the highest average of prices where where “Roxhill” is the neighborhood that has the lowest average of prices. The list below shows the top 5 neighborhoods and the low 5 neighborhoods according to the average of prices.
Top 5 neighbourhoods :

Neighborhood          price
                  
Fairmount Park       370.000000
Industrial District  245.000000
Portage Bay          241.428571
Westlake             197.000000
Alki                 196.652174


 Low 5 neighbourhoods :

neighbourhood   price
           
Roxhill        60.000000
Olympic Hills  63.666667
Dunlap         71.750000
Rainier Beach  76.722222
Georgetown     77.000000


