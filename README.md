# Funnel-Analysis-
Funnel analysis is a method of data analysis used to track and understand the sequential steps or stages that users or customers go through when interacting with a product, service, or website.

# TLDR
## Recommendation

- Onboarding Optimization
- Enhance User Experience for Ride Completion
- Encourage Reviews Post-Payment
- Platform-Specific Marketing Focus
- Age-Targeted Campaigns
- Engage Users with Unspecified Age
- Optimize User Experience for Web Platform
- Leverage Review Opportunities on Android
- Capitalizing on Peak Demand Hours
- Consider External Factors

# Table of Contents
-[SUMMARY](#summary)

-[FUNNEL RESULTS](#funnel-results)

-[Platform Distribution Over User Funnel](#platform-distribution-over-user-funnel)

-[Age Range Distribution Over User Funnel](#age-range-distribution-over-user-funnel)

-[Ride Request Distribution Through the Day](#ride-request-distribution-through-the-day)

-[Recommendation and Conclusion](#recommendation-and-conclusion)

-[SQL Appendix](#sql-appendix)
  
-[Tableau Dashboard](#tableau-dashboard)

# SUMMARY

The project focused on understanding and improving the user funnel, encompassing key stages from app download to ride review. Our goal was to identify areas for enhancement and optimization. The customer funnel comprises seven stages, starting from app download to review. Drop-offs occur at various stages, necessitating funnel analysis for improvement. Business questions revolve around key aspects like drop-off points, platform performance, age group preferences, surge pricing, and low conversion areas.

![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/Funnel%20Steps.png)

# FUNNEL RESULTS
## User Level 
- Download to Signup (Drop-off: 25.49%): This stage has a 25.49% drop-off rate, indicating that approximately a quarter of users who download the app do not proceed to sign up. This could be due to various factors such as a cumbersome signup process, unclear value proposition, or technical issues.
- Signup to Rides Requested (Drop-off: 29.53%): There is a further drop of 29.53% from signup to rides requested. This indicates that nearly a third of users who sign up do not proceed to request a ride. Possible reasons could include concerns about ride availability, pricing, or user interface issues.
- Rides Requested to Rides Accepted (Drop-off: 0.21%): This stage has a very low drop-off rate, indicating that the vast majority of users who request a ride have their request accepted by a driver. This suggests that the platform effectively matches ride requests with available drivers.
- Rides Accepted to Rides Completed (Drop-off: 48.2%): The highest drop-off occurs between the "Rides Accepted" and "Rides Completed" stages. This indicates a significant challenge in getting accepted rides to reach completion, which is a critical point for user satisfaction.
- Rides Completed to Payment (Drop-off: 0%): There is no drop-off at this stage, indicating that all users who complete a ride proceed to the payment stage. This is an excellent conversion rate and suggests that users are comfortable with the payment process.
- Payment to Review (Drop-off: 30.17%): This stage has a drop-off of 30.17%, indicating that about a third of users who make a payment do not leave a review. This could be due to various reasons, including user preference, lack of incentive, or oversight.

![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/User%20Funnel.png)

##  Ride Level:
- Download and Signup: These stages don't involve rides, so there are no drop-offs at these points.
- Rides Requested: This stage sees a total of 385,477 ride requests. There are no drop-offs at this point, indicating strong user engagement in requesting rides.
- Rides Accepted: From the ride requests, 248,379 rides are accepted, indicating a 64.43% conversion rate. However, there's a drop-off of 35.57% at this stage. This drop-off suggests that there may be room for improvement in the acceptance process.
- Rides Completed: Of the accepted rides, 223,652 are completed, indicating a 90.04% conversion rate from accepted to completed rides. There is no drop-off at this stage, indicating a smooth process once a ride is accepted.
- Payment: 212,628 rides result in payments, which is a 95.07% conversion rate from completed rides to payments. There is no drop-off at this stage, suggesting that users are comfortable with the payment process.
- Review: Finally, 156,211 rides lead to reviews, indicating a 73.47% conversion rate from payments to reviews. There's a drop-off of 21.6% at this stage, indicating that there may be room to encourage more users to leave reviews after making payments.

![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/Ride%20Funne.png)

# Platform Distribution Over User Funnel

## iOS Platform Dominance:
The data indicates that a significant portion of Metrocar’s user base prefers the iOS platform. This could be attributed to factors such as user preferences, brand loyalty, or the perception of a seamless experience on iOS devices. As a result, it’s crucial to continue optimizing the Metrocar app for iOS to cater to this large user segment.
## Impressive Signup Conversion on iOS:
Among the different platforms, iOS users exhibit the highest signup conversion rate at an impressive 75.07%. This indicates that a substantial proportion of iOS users who download the app proceed to complete the signup process. This suggests that the onboarding experience on iOS devices is particularly effective, potentially due to an intuitive interface or a well-structured signup flow.
## Challenges on the Web Platform:
The web platform, while essential for providing accessibility to users without dedicated mobile apps, presents a notable challenge. The completion rate for ride requests on the web platform experiences a drop-off of 49.8%. This suggests that there may be usability issues or friction points specific to the web interface that lead to a higher rate of users abandoning the ride request process. Addressing these issues could significantly improve the conversion rate on the web platform.

![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/Android.png)
![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/IOS.png)
![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/Web.png)

# Age Range Distribution Over User Funnel

## Performance of the 35-44 Age Group:
The age group of 35–44 demonstrates the highest performance throughout the user funnel. This means that individuals in this age range are more likely to progress through the stages of the app, from download to completing rides and leaving reviews. They constitute a significant portion of Metrocar's user base, indicating that this demographic is particularly engaged with the service.
## Unspecified Age Information:
Users with unspecified age information account for 30% of the total signed-up user base. This is a substantial portion, and it's crucial to understand and potentially address why this information is missing. It may be due to a variety of reasons, such as user privacy preferences or technical issues during registration. Investigating and encouraging users to provide their age could lead to a more comprehensive understanding of the user base.
## Challenges for the 25-34 Age Group on the Web Platform:
Within the 25-34 age range, users utilizing the web platform experience the most significant drop-off in completing rides, standing at 46.7%. This indicates a notable challenge specific to this age group and platform combination. It suggests that there may be usability or functionality issues on the web platform that need attention to improve the ride completion rate for users in this demographic.
## Reviews from the 45-54 Age Group on Android:
On the Android platform, users aged 45–54 exhibit the highest likelihood of leaving reviews, with an impressive 75.27% conversion rate. This is a positive sign, indicating that this demographic is actively engaged in providing feedback. Understanding why this age group is more inclined to leave reviews can provide valuable insights for encouraging reviews from other user segments.

![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/18-24.png)
![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/25-34.png)
![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/35-44.png)
![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/45-54.png)

# Ride Request Distribution Through the Day

- The histogram provides a clear visual representation of the hours with the highest demand for rides. Notably, there are two distinct surges in ride requests. The first surge occurs in the morning between 8-10 a.m., suggesting that a significant portion of users rely on Metrocar for their daily work commute. This influx of ride requests is likely attributed to rush-hour traffic and the need for a convenient and reliable transportation option.
- The second surge takes place in the late afternoon to early evening, spanning from 4 to 7 PM. This pattern indicates another peak period of demand, which aligns with individuals starting their journeys back home after work or other daytime commitments. This trend is common among urban commuters seeking efficient transportation options during peak traffic hours.
Moreover, these time slots may also align with standard work hours and school schedules, contributing to the increased demand for rides during these specific time frames. It's essential to consider the impact of these routines on the demand for Metrocar services, as they play a pivotal role in shaping user behavior and preferences.
- Additionally, external factors such as traffic patterns and public transportation schedules may further amplify the observed spikes in ride requests. Understanding and adapting to these patterns can help Metrocar optimize its services to meet the high demand during these crucial time frames.
![alt text](https://github.com/Fitasdj/Funnel-Analysis-/blob/main/Ride%20Request%20Distribution.png)

# Recommendation and Conclusion
### Onboarding Optimization:
Streamline the signup process to reduce the 25.35% drop-off observed after app downloads.
### Enhance User Experience for Ride Completion:
Address the 48.2% drop-off in the 'Rides Completed' stage. Investigate and implement improvements to ensure seamless ride completion.
### Encourage reviews post-payment: 
Leverage the 30.24% drop-off at the 'Payment to Review' stage as an opportunity to encourage more users to leave reviews after making payments.
### Platform-Specific Marketing Focus:
Given that the majority of users prefer iOS, allocate the marketing budget accordingly. Additionally, consider targeted strategies to address the 49.8% drop-off rate for completed ride requests on the web platform.
### Age-Targeted Campaigns:
Tailor marketing efforts towards the 35–44 age group, which demonstrates the highest performance throughout the user funnel.
### Engage Users with Unspecified Age:
As users with unspecified age information make up 30% of the signed-up user base, consider initiatives to gather and engage with this demographic.
### Optimize User Experience for Web Platforms:
Within the 25-34 age range, users on the web platform experience a 46.7% drop-off in completing rides. Focus on enhancing the user experience for this segment.
### Leverage Review Opportunities on Android:
Users aged 45–54 on the Android platform show a high likelihood of leaving reviews (75.27% conversion rate). Encourage and incentivize reviews from this demographic.
### Capitalizing on Peak Demand Hours:
Maximize resources during peak demand hours of 8–10 a.m. and 4–7 p.m. Consider adjusting driver schedules and incentives to meet increased ride requests during these times.
### Consider External Factors: 
Factor in external elements like traffic patterns and public transportation schedules that may contribute to the observed spikes in ride demand during specific hours.

# SQL Appendix
## SQL Query to Construct the Funnel:
```
SELECT * FROM ( WITH q AS (
SELECT DISTINCT CAST ((DATE_TRUNC ('DAY', download_ts)) AS DATE) AS download_dt,
app_download_key,
user_id,
ride_id,
transaction_id,
review_id,
age_range,
platform,
request_ts,
driver_id,
dropoff_ts,
charge_status
FROM metrocar
ORDER BY 1)
SELECT 0 AS funnel_step, 'download' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT app_download_key) AS user_count,
0 AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL

SELECT 1 AS funnel_step,
'signup' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT user_id) AS user_count,
0 AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL

SELECT 2 AS funnel_step,
'ride_requested' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT CASE WHEN ride_id IS NOT NULL THEN user_id END ) AS user_count,
COUNT(ride_id) AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL

SELECT 3 AS funnel_step,
'ride_accepted' AS funnel_name,
download_dt,
age_range,
 platform,
COUNT(DISTINCT CASE WHEN driver_id IS NOT NULL THEN user_id END ) AS user_count,
COUNT(CASE WHEN driver_id IS NOT NULL THEN ride_id END) AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL

SELECT 4 AS funnel_step,
'ride_completed' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT CASE WHEN dropoff_ts IS NOT NULL THEN user_id END ) ASuser_count,
COUNT(CASE WHEN dropoff_ts IS NOT NULL THEN ride_id END ) AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL

SELECT 5 AS funnel_step,
'payment' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT CASE WHEN charge_status = 'Approved' THEN user_id END ) AS user_count,
COUNT(CASE WHEN charge_status = 'Approved' THEN ride_id END ) AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL

SELECT 6 AS funnel_step,
'review' AS funnel_name,
download_dt,
age_range,
platform,
COUNT (DISTINCT CASE WHEN review_id IS NOT NULL THEN user_id END ) AS user_count,
COUNT (CASE WHEN review_id IS NOT NULL THEN ride_id END) AS ride_count
FROM q
GROUP BY 3,4,5
ORDER BY 5,4,3) sub
ORDER BY funnel_step ASC
```
## SQL Query to Calculate Percent of Top and Percent of Previous:
```
WITH q1 AS (
WITH cte1 AS (
SELECT funnel_step,
funnel_name,
SUM(user_count) AS total_users,
LAG(SUM(user_count)) OVER() AS user_previous_value,
FIRST_VALUE(SUM(user_count)) OVER()AS user_top_value,
SUM(ride_count) AS total_rides,
LAG(SUM(ride_count)) OVER() AS ride_previous_value
FROM ( WITH q AS (
SELECT DISTINCT CAST ((DATE_TRUNC ('DAY', download_ts)) AS DATE) AS download_dt,
app_download_key,
user_id, ride_id,
transaction_id,
review_id,
age_range,
platform,
request_ts,
driver_id,
dropoff_ts,
charge_status
FROM metrocar
ORDER BY 1)
SELECT 0 AS funnel_step,
'download' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT app_download_key) AS user_count,
0 AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL
SELECT 1 AS funnel_step,
'signup' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT user_id) AS user_count,
0 AS ride_count
FROM q
GROUP BY 3,4,5


UNION ALL
SELECT 2 AS funnel_step,
'ride_requested' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT CASE WHEN ride_id IS NOT NULL THEN user_id END ) AS user_count,
COUNT(ride_id) AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL
SELECT 3 AS funnel_step,
'ride_accepted' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT CASE WHEN driver_id IS NOT NULL THEN user_id END ) AS user_count,
COUNT(CASE WHEN driver_id IS NOT NULL THEN ride_id END) AS ride_count
FROM q
GROUP BY 3,4,5


UNION ALL
SELECT 4 AS funnel_step, 'ride_completed' AS funnel_name, download_dt,
age_range, platform,
COUNT(DISTINCT CASE WHEN dropoff_ts IS NOT NULL THEN user_id END ) AS
user_count,
COUNT(CASE WHEN dropoff_ts IS NOT NULL THEN ride_id END ) AS ride_count FROM q
GROUP BY 3,4,5


UNION ALL
SELECT 5 AS funnel_step,
'payment' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT CASE WHEN charge_status = 'Approved' THEN user_id END ) AS user_count,
COUNT(CASE WHEN charge_status = 'Approved' THEN ride_id END ) AS ride_count
FROM q
GROUP BY 3,4,5

UNION ALL

SELECT 6 AS funnel_step,
'review' AS funnel_name,
download_dt,
age_range,
platform,
COUNT(DISTINCT CASE WHEN review_id IS NOT NULL THEN user_id END ) AS user_count,
COUNT(CASE WHEN review_id IS NOT NULL THEN ride_id END ) AS ride_count
FROM q
GROUP BY 3,4,5
ORDER BY 5,4,3) sub
GROUP BY 1,2
ORDER BY 1)

SELECT
funnel_step,
funnel_name,
total_users,
user_previous_value,
user_top_value,
total_rides,
ride_previous_value,
--ride_top_value,
ROUND((100*total_users / user_previous_value),2) AS user_per_of_previous, ROUND((100*total_users/first_value(total_users) OVER()),2) AS user_per_of_top, CASE WHEN total_rides != 0 AND ride_previous_value != 0 THEN
ROUND((100*total_rides / ride_previous_value),2) ELSE 0 END AS ride_perc_of_previous


FROM cte1 ),
q2 AS ( SELECT *,
MAX(total_rides) OVER() ride_top_value FROM q1
)

SELECT q1.funnel_step,
q1.funnel_name,
q1.total_users,
q1.user_previous_value,
q1.user_top_value,
q1.total_rides,
q1.ride_previous_value,
FIRST_VALUE(ride_top_value) OVER() AS ride_top_value,
ROUND((100*q1.total_users / q1.user_previous_value),2) AS user_per_of_previous,
ROUND((100*q1.total_users/first_value(q1.total_users) OVER()),2) AS user_per_of_top,
CASE WHEN q1.total_rides != 0 AND q1.ride_previous_value != 0 THEN ROUND((100*q1.total_rides / q1.ride_previous_value),2) ELSE 0 END AS ride_perc_of_previous,
ROUND((CASE WHEN q1.total_rides != 0 THEN 100 * q1.total_rides / FIRST_VALUE(ride_top_value) OVER() ELSE 0 END),2) AS ride_perc_of_top
FROM q1
LEFT JOIN q2 ON q1.funnel_step = q2.funnel_step
```
# Tableau Dashboard
URL: https://public.tableau.com/app/profile/djamel.fitas/viz/MetrocarFunnelAnalysis_16983605038720/MetrocarFunnelAnalysis

