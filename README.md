# SuperstoreProjectFile-2
This file contains SQL queries for our project. In this stage, I'd like to Arda Kantık to help me to write those queries. We've found that Superstore hasn't got any null values for each column. Then we've removed one duplicated row in the dataset and copied it into new table. This was our dataset based on OrderId. We've checked our columns types by using INFORMATION_SCHEMA.COLUMNS.

In this dataset, the columns called sales,quantity and profit were the most important columns for us so, we've handled outliers for these columns. We've tried to remove outliers first for these columns but we've realized that we've removed %30 of dataset :). This was too much percantage to get rid of outliers directly, so we've capped our outliers instead. Thanks for Sine Gökhan's outlier analysis in Python, we've found that %5 - %95 for lower and upper limit was the best limits for capping process. Then we've performed capping process in the SQL.

Then we've performed data enriching. We've added new columns. ThisOrdersDayDiff shows daydiff between OrderDate and ShipmentDate for a single order. OrderYear shows OrderDate's year. Revenue shows 
