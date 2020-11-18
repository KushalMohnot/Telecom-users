# Telecom-users
Data description: The data is from 500 Megaline clients: who the clients are, where they're from, which plan they use, and the number of calls they made and text messages they sent in 2018. 

Five files: calls, internet, messages, plans, users. Attributes described below:

The users table (data on users):
user_id — unique user identifier
first_name — user's name
last_name — user's last name
age — user's age (years)
reg_date — subscription date (dd, mm, yy)
churn_date — the date the user stopped using the service (if the value is missing, the calling plan was being used when this database was extracted)
city — user's city of residence
plan — calling plan name
The calls table (data on calls):
id — unique call identifier
call_date — call date
duration — call duration (in minutes)
user_id — the identifier of the user making the call
The messages table (data on texts):
id — unique text message identifier
message_date — text message date
user_id — the identifier of the user sending the text
The internet table (data on web sessions):
id — unique session identifier
mb_used — the volume of data spent during the session (in megabytes)
session_date — web session date
user_id — user identifier
The plans table (data on the plans):
plan_name — calling plan name
usd_monthly_fee — monthly charge in US dollars
minutes_included — monthly minute allowance
messages_included — monthly text allowance
mb_per_month_included — data volume allowance (in megabytes)
usd_per_minute — price per minute after exceeding the package limits (e.g., if the package includes 100 minutes, the 101st minute will be charged)
usd_per_message — price per text after exceeding the package limits
usd_per_gb — price per extra gigabyte of data after exceeding the package limits (1 GB = 1024 megabytes)
Things to explore:
Describe the customers' behavior. Find the minutes, texts, and volume of data the users of each plan require per month. Calculate the mean, variance, and standard deviation. Plot histograms. Describe the distributions.
For each user, find:
The number of calls made and minutes used per month
The number of text messages sent per month
The volume of data per month
The monthly profit from each user (subtract the free package limit from the total number of calls, text messages, and data; multiply the result by the calling plan value; add the monthly charge depending on the calling plan)
Possible hypothesis tests: 
The average profit from users of Ultimate and Surf calling plans differs.
The average profit from users in the NY-NJ area is different from that of the users from other regions.
 

