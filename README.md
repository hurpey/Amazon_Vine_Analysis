# Amazon_Vine_Analysis

**Overview:**

The purpose of this project is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

This project uses PySpark to perform the ETL process to extract dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin, for approximately 50 datasets. Each dataset contains reviews of a specific product, from clothing apparel to wireless products. The project also uses PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in the dataset. 


**Results:**

Below are some snapshots of dataframe from the Amazon Vine analysis:

<img width="851" alt="final vine table df" src="https://user-images.githubusercontent.com/79670933/122697723-f0bc0e80-d213-11eb-93bc-e904c45dd48f.png">

<img width="60<img width="508" alt="dataframe" src="https://user-images.githubusercontent.com/79670933/122699873-3d094d80-d218-11eb-9732-abe48339abf0.png">


The images below show a snapshot of the comparison of the vine and non-Vine reviews. 

<img width="400" alt="vine reviews" src="https://user-images.githubusercontent.com/79670933/122698253-ee0de900-d214-11eb-9ac3-3e070cbece8d.png">
<img width="600" alt="All reviews" src="https://user-images.githubusercontent.com/79670933/122700113-a8531f80-d218-11eb-90ee-3a0e3bfa84c8.png">
<img width="600" alt="all non vine reviews" src="https://user-images.githubusercontent.com/79670933/122698007-7a6bdc00-d214-11eb-83c0-4e3f367f276b.png">
<img width="400" alt="non vine reviews" src="https://user-images.githubusercontent.com/79670933/122697764-03cede80-d214-11eb-8504-dcc1349ff324.png">
<img width="400" alt="all 5 star furniture review" src="https://user-images.githubusercontent.com/79670933/122697767-04677500-d214-11eb-9d8a-bec76534e40f.png">
<img width="400" alt="All furniture reviews" src="https://user-images.githubusercontent.com/79670933/122697768-04677500-d214-11eb-82e3-573761620881.png">
<img width="400" alt="all vine product reviews" src="https://user-images.githubusercontent.com/79670933/122697770-04677500-d214-11eb-8484-599981727900.png">

Based on the analysis perfromed and snapshots above, the following are observed:

- There are 2,775 Vine reviews and 789,338 non-Vine reviews.

- There are 1,356 "5-Star" Vine reviews and 446,360 "5-Star" non-Vine reviews.

- 48.9% of all Vine reviews are "5 Star". 56.5% of non-Vine reviews are "5-Star".


**Summary:**

In summary, we can see that most of the reviews  for Furniture product are almost nothing or lower results from non vine reviews. Also, more of the non -Vine reviews are 5 star ratings. Additional analysis that can be performed will be looking at the percentage of rating by stars (that is, 1 star to 5 star) asshown in the image below. From this analysis, we can see that more than 80% of favorable responses are 4 stars and above.

<img width="400" alt="vine reviews" src="https://user-images.githubusercontent.com/79670933/122699568-a046b000-d217-11eb-977b-fdc4718c1c79.png">
