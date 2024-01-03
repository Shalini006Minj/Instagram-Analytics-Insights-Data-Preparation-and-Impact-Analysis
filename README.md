## Introduction
This document provides a detailed examination of the data preparation, cleaning, and manipulation process for Instagram analytics. It focuses on methods for restructuring data columns, consolidating datasets, and calculating key metrics such as total followers and growth rates. The analysis includes a thorough examination of content stats, including retention and engagement rates, and a comparison of different types of Instagram posts. The document also explores the relationships between various metrics to understand their impact on Instagram's reach and follower dynamics, offering recommendations for content strategy based on these insights.

## Objective
To design a data-driven Instagram engagement analysis dashboard to gain insights into the performance of different post types on Data Analyst Duo's Instagram account (@dataanalystduo) with approximately 106,000 followers.

![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/414c3159-b7ba-4af8-9a96-d1e5e6d2e57a)

## Data Preparation, i.e. Cleaning and Manipulation
•	Date Column Restructuring: The date column under the "Reach," "Profile visits," and "New followers" sheets was manipulated using the TEXT TO COLUMN delimiter 
  "T," as shown below
      
•	Consolidation of Dataset: 

    -Two separate datasets, "Followers Stats" and "Content Stats," were created
    -For a cohesive analysis, we concentrated on the period that began on December 1, 
     2022, which aligned with the commencement date of the content statistics 
     datasets and offered a consistent timeline for both datasets
      
•	Total Followers Calculation:

    -For this step, we added the total of women and men, which came up to ‘106031’
    -Next step involved subtracting 106031 from the sum of new Instagram followers, 
     which gave the value for 01-Dec-2022 i.e. ‘13845’ 
    -The calculation of 'Total Followers' for each following day involved the summation 
     of the 'New Instagram Followers' for that particular day. 
    -It's important to note that this calculation excluded unfollows to maintain 
     accuracy, as considering them could result in a minor fluctuation in the 
     follower’s count.
     
•	Growth Rate Calculation:

    -This calculation involves dividing the number of followers gained on the current 
     day by the number of followers gained on the previous day
    -The purpose of this calculation is to track the daily growth or change in followers, 
     providing valuable insights into the rate of audience expansion over time.
    
•	Analysis of Content Stats:

    -Retention Rate - It is determined by dividing the number of '3s views' by the total number 
     of 'impressions' for each post. This calculation is performed to 
     assess how effectively a post engages the audience and retains their attention.
    -Engagement Rate – We sum the total number of 'likes,' 'comments,' 'saves,' and 'shares' on a daily basis
     and then divide this sum by the daily post's reach.       
    -The reason for calculating this metric is to assess the engagement rate of posts 
     on a daily basis. This helps us to understand how effective the content is 
     in terms of attracting interaction from the audience relative to the reach it achieves.
    -Duration Bins – The primary objective behind this action was to classify the time span of 
    posts into two distinct categories: "more than 30 seconds" and "less than or equal to 30 seconds."

## Analysis and Insights
•	Instagram Reach:
![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/cdd5f2d0-96da-4d8a-80ea-68a5bd59eaac)

The similarity in patterns for both years could indicate a trend that aligns with seasonal or periodic events that affect Instagram reach. 

Instagram's algorithm tends to favor consistency in posting, user engagement, and content relevance. 

If the content strategy was similar during both years, that could explain the consistent patterns of reach

The spike observed in May and June 2023, contrasting with the lowest reach in the same months in 2022, could be due to several factors:

     o Content Shifts: There may have been a shift in the content strategy run during these months in 
       2023 that resonated well with the audience.
     o Platform Algorithm Changes: Instagram periodically updates its algorithm, and these updates can 
       dramatically affect reach. Perhaps there was an update that favored the type of content that was 
       published at the time.
     o Viral Content: It's possible that some content posted in May and June 2023 went viral, which would 
       significantly escalate the reach.
     o Increased User Engagement: There could have been a surge in user engagement due to interactive content 
       or trends that the account participated in.
       
•	Instagram Followers Visit:
![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/d692de2f-7c42-4eb3-907a-7ee96d927df8)

The significant rise in visits during May 2023 may be attributed to one or more posts gaining viral traction, which in turn enhanced overall visibility and attracted a higher number of visits.

A consistent decline in followers' visits and reach is observed from June through September 2023. This trend could indicate that the audience may be experiencing fatigue, potentially due to a decrease in content quality or an excessive quantity of posts.

Shifts in audience preferences or behaviors could also lead to lower engagement as seen in March, October and September 2023.

•	Comparison Analysis:
![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/1876ab10-087e-4957-be2b-4ad9fbc52b77)

![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/de588722-8ee5-415e-a59e-7f9a7737a901)

![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/ad7c0a61-e683-4b68-8614-afbeea86b270)

Instagram reach and Instagram follower's visits are two interconnected metrics that are significantly impacting each other. 

The graphs depicting Instagram reach and Instagram followers’ visits exhibit parallel trends, likely influenced by the platform's algorithm that prioritizes content with high engagement, which is measured through likes, comments, and shares. As the reach of a post escalates, it becomes more visible to a wider audience, consequently spurring an increase in profile visits as users engage with the content they encounter.

Another reason for the similar trend could be the use of Instagram Live sessions to engage with the audience in real time, which can increase reach and prompt viewers to visit the profile.

New Instagram followers are showing divergence in trends from the above two graphs, as not all users who interact with content or visit a profile are inclined to follow. They may need repeated exposure or a particular type of content to make that commitment.

The observed spike in new followers during December 2022 and January 2023, without a proportional rise in profile visits, may suggest that certain content resonated widely, going viral beyond the usual audience. This would lead to a surge in followers who engaged directly with the viral posts, bypassing the necessity to view the profile page.

This spike could also be the reason for change in new year goals or resolution as some users may be exploring new interests and following accounts that align with goals.

•	Relationship Analysis:
![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/d11f27e9-2662-4c5a-aebf-aa8b8bce4016)

Based on the scatter plot it is evident that there is a positive correlation between Instagram reach and Instagram followers' visits. 

This means that as the reach increases, there is a tendency for the number of visits from followers to increase as well. 

However, there are some data points that show high reach but comparatively lower follower visits, indicating that there could be other factors at play affecting the relationship between these two metrics.

Here are some insights and recommendations based on the data and graph:

    o Hashtag Use: By employing relevant hashtags to improve the discoverability of the posts. Hashtags can 
      significantly increase reach beyond the existing       
      followers, and if they are targeted correctly, they can attract more visits from interested users.
    o Posting Schedule: By analyzing the times, the followers are most active and scheduling the posts accordingly can 
      help in getting immediate engagement, which can boost the post's reach and result in more visits.

Note that while a direct correlation can be observed, the quality of engagement is more critical than the quantity. It’s not just about reaching a broad audience but reaching the right audience that is interested in and interacts with your content.

•	Correlation Analysis in Content Stats				
![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/3b791512-ed8c-46d9-ad5d-73c7f29a2e6a)

The analysis was conducted to determine the correlation between various metrics, such as likes, comments, shares, and others. 

The purpose of this analysis was to understand the relationships between these metrics that can provide valuable Instagram insights.

Some insights can be drawn are as follows:

    o Impressions & Reach: Highly correlated (0.998), suggesting that as the number of times a post is displayed (impressions) increases, 
      its reach also increases.
    o Shares, Follows, & 3s Views: These also show strong positive correlations with Impressions and Reach, indicating that more popular posts 
      tend to get shared more and attract more followers and views.
    o Likes: Strongly correlated with Impressions (0.963) and Reach (0.955), suggesting that posts with higher visibility tend to get more likes.
    o Comments: Moderately correlated with other metrics, indicating that while higher visibility leads to more comments, the relationship is not 
      as strong as with likes or shares.
    o Saves: Highly correlated with Shares (0.964), indicating that posts that are shared more are also saved more frequently.

•	Engagement Across Different Types of Posts:
![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/ef311127-fd95-4ff0-ac5b-f5b971ef060e)

The provided image shows a table, which compares the engagement metrics across three different types of Instagram posts: IG carousel, IG image, and IG reel.

Post Type: The most common type of post was the IG reel, with 127 descriptions, followed by IG carousel (25) and IG image (16). This suggests that IG reels are the most frequently posted content type in this dataset. 

Reach and Impressions: IG reels have the highest average reach (52,065) and impressions (58,707), indicating they are seen by more unique users and more often than the other post types.

Engagement Metrics (Shares, Likes, Comments, Saves):

    o Shares: IG reels are shared significantly more (680) on average than carousels (256) and images (72).
    o Likes: IG reels also have the highest number of average likes (1,915), followed by IG carousel (1,338) and IG image (953).
    o Comments: IG carousel posts receive the most comments on average (72), followed by reels (38) and images (21).
    o Saves: IG reels are saved more often (2,178) than IG carousels (1,668) and IG images (557).

Engagement Rate: IG carousel posts have the highest average engagement rate (9%) when considering reach, followed by IG reels (8%) and IG images (5%). This suggests that while reels reach more people, carousels engage a higher proportion of their audience.

Retention Rate: The retention rate is only provided for IG reels (56%), which is a strong indicator that more than half of the viewers returned to view the content again. This metric is 0% for both IG carousels and IG images, which could indicate that the data is missing, or these post types did not bring back viewers.

Insights:

      o IG Reels seem to be the most effective in terms of reach, shares, likes, and saves, which indicates their 
        format is likely more engaging and favored by the Instagram algorithm. The retention rate for reels is outstanding, 
        showing they are quite effective in keeping the audience's interest to re-watch the content.
      o IG Carousel posts, despite being less in number, have the highest engagement rate relative to their reach, which 
        suggests that they are quite effective in engaging the audience who sees them.
      o IG Images appear to be the least engaging across all metrics but still maintain a decent average number of likes.

 •	Engagement Across Duration (>30 secs & <=30 secs)     
 ![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/f24f96c9-2f87-43fe-bc9f-a0473b855ba6)

The analysis focuses on the engagement metrics for Instagram reels based on their duration, categorizing them into two groups: reels that are less than or equal to 30 seconds and reels that are more than 30 seconds.

Count of Description: There were more reels with a duration of more than 30 seconds (77) compared to those 30 seconds or less (50), suggesting a preference or strategy for longer content.

Reach and Impressions: Shorter reels (≤30 secs) have a higher average reach (59,003) and impressions (64,637) than longer reels (>30 secs), which means they are seen by more unique users and more often.

Shares: Longer reels are shared slightly more (710) on average than shorter ones (634), which might indicate that viewers find the longer content more share-worthy.

Likes and Saves: Shorter reels receive more likes (1,864) and saves (2,298) on average compared to longer reels (1,948 likes and 2,101 saves). This indicates that while the difference is not large, shorter reels tend to be slightly more favored by users in terms of liking and saving the content.

Comments: Shorter reels also receive more comments (49) on average than longer ones (30), suggesting higher user interaction.

Engagement Rate: Despite having a lower reach, longer reels have a higher average engagement rate (8%) compared to shorter ones (7%). This suggests that the audience for longer reels is more engaged relative to the number of people reached.

Retention Rate: Shorter reels have a higher retention rate (61%) compared to longer reels (52%), meaning a greater percentage of viewers return to watch shorter reels again.

Insights:

    o Shorter reels seem to perform better in terms of reach, impressions, likes, comments, saves, and retention rate. This suggests 
      that the platform's users have a preference for shorter, more digestible content.
    o Longer reels, while not performing as well in reach or retention, do engage their audience at a slightly higher rate once reached. 
      This could indicate that viewers who prefer longer videos are more committed to engaging with the content.
    o Content creators should consider maintaining a mix of both shorter and longer reels to maximize reach and engagement. Shorter reels 
      might be used to attract and retain viewers, while longer reels could foster deeper engagement with a potentially more invested audience.
    o The preference for shorter or longer content might also depend on the nature of the content itself, and as such, creators 
      should tailor the length of their reels to the message or story they are conveying.

•	Word Cloud Analysis:
![image](https://github.com/Shalini006Minj/Instagram-Analytics-Insights-Data-Preparation-and-Impact-Analysis/assets/138965178/cb50332d-c17b-408a-bde0-3f47911b86e0)

The analysis shows that by focusing on popular and relevant keywords such as "data," "analytics," "SQL," and "Python," is appealing to the interests of the target audience. High-value content like tutorials, tips, industry insights, and thought leadership articles around these topics can attract followers.

Hashtags like #DataScience, #DataAnalytics and #Python, in the posts is increasing the visibility of the content on Instagram, making it discoverable to users interested in these topics.

Consistent use of the terms "dataanalystduo" and “datatodestiny” is helping the creator to strengthen their brand identity on Instagram. It is creating a recognizable presence that resonates with their audience and building brand loyalty.

## Recommendations

Words like "follow," "comment," and "trending" suggest a strategy focused on engaging with the community. Encouraging followers to engage with your content through comments, shares, and likes can increase engagement rates, which are vital for growth on Instagram.

The spike in reach observed in May and June 2023 could be attributed to viral content. Creators can consider creating content that resonates well with the audience and has the potential to go viral. 

Creators can emphasize more on creating short reels (<= 30secs) which will talk about learning resources, valuable certifications, and project ideas can help building a highly engaging audience. This could include course recommendations, certification guides, project showcases, and study tips.








       



