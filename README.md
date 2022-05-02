# ExpediaHotelRecommendation
Team Project for CMPE 256

We are developing a Hybrid Collaborative Recommedation for Expedia Hotel. This hotel recommendation system will recommend a group of hotels to the users based on their prior actions or previous hotel bookings. The goal of this project is to predict the booking outcome (hotel cluster) for a user event, based on their search and other attributes associated with that user event. 

**Dataset descriptions**

**train.csv** - the training set
**test.csv** - the test set
**destinations.csv** - hotel search latent attributes

**train.csv/test.csv Data fields:**

Column name									Description															Data type

date_time										Timestamp																string

site_name										ID of the Expedia point of sale 				int

posa_continent							ID of continent associated 							int

user_location_country				The ID of the country the customer 			int

user_location_region				The ID of the region the customer 			int

user_location_city					The ID of the city the customer 				int

orig_destination_distance		Physical distance 											A null means the distance could not be calculated	double

user_id											ID of user															int

is_mobile										1 when a user connected, 0 otherwise		tinyint

is_package									1or 0																		int

channel											ID of a marketing channel								int

srch_ci											Checkin date														string

srch_co											Checkout date														string

srch_adults_cnt							The no. of adults in the hotel room			int

srch_children_cnt						The no. of children  in the hotel room	int

srch_rm_cnt									The no. of hotel rooms in the search		int

srch_destination_id					ID of the destination 									int

srch_destination_type_id		Type of destination											int

hotel_continent							Hotel continent													int

hotel_country								Hotel country														int

hotel_market								Hotel market														int

is_booking									1 if a booking, 0 if a click						tinyint

cnt													Numer of similar events 								bigint

hotel_cluster								ID of a hotel cluster										int

**destinations.csv Data fields**

Column name									Description															Data type

srch_destination_id					ID of the destination 									int

d1-d149											latent description of search regions		double

