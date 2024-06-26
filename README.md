# Social Media Growth Strategy Project

## Executive Summary

Our content strategy balances **daily single posts (1-2)** with **weekly threads (3-5)**, ensuring a steady stream of updates while diving deeper into significant topics. However, October marked a pivotal moment with a **43% decline in total impressions**, highlighting the n**eed to reassess our approach to content and audience engagement dynamics**. Further analysis unveiled **threads as the engagement frontrunners**, boasting nearly double the interaction rates compared to single posts, and significantly outperforming in profile clicks and follower acquisition.

Moving forward, my recommendations **pivot on increasing thread-centric content from both a quantity and quality point of view as an immediate priority. **

## Project Overview

The aim of this project is to analyse Twitter/X data to determine the best social media strategy for profile reach and growth. I’ll be looking specifically at which type of content - threads versus single posts - drives the most engagement from users on the platform. I’ll analyse tweet data to investigate the engagement rate of each post depending on its format and topic using Excel and Power Query. My objective is to understand the relationship between the type of post (single or thread) and the level of engagement it receives. What I learn will then guide our social media content planning for better engagement. This project will provide me with empirical evidence on which to base our future social media strategies, thus putting us in a stronger position to grow my audience on Twitter/X.

## Data Sources

For this project I will be using a CSV export of all my tweets from 1st October 2023 – 31st October 2023. CSV files are a simple, widely accepted, and easy-to-understand data format. Being text files, they are human-readable and lightweight making them excellent for exporting small to medium datasets from platforms such as Twitter. However, they have limitations. CSV files lack a standard schema, making interpretation of data more difficult across different systems. They also require manual export and can become inefficient with large amounts of data.

If the outcomes of my project prove significant, it might be worth considering the development of a data pipeline using Twitter's API instead. This would also allow us to extract more data in real-time and potentially access more detailed data. The main benefits include scalability, ease of use and improved access to information which could open new doors for my data analysis and project potential.

## Data Cleaning & Transformation

I loaded the CSV file extracted from the Twitter platform into Power Query. I promoted the headers on the data table for better comprehension and corrected the inferred data types to match the nature of information they hold, such as converting "Tweet ID" and "impressions" into integers and "time" into datetime. Next, I removed any columns that were not needed for my analysis, such as "Tweet id", "URL clicks", "hashtag clicks" and others related to promoted content. This makes my data model leaner and more manageable. From my tweet text, I excluded entries that contained "@" (replies to other twitter users) or "here:" (promotional tweets), as they might have skewed the results.

The next challenge I faced was how to determine which tweets were part of a thread and which were single posts. I decided to group tweets by their posting date & time assuming that any tweet posted at the same day/time can be considered a thread and anything else can be considered a singular post. I duplicated the cleaned dataset and aggregated my data accordingly. Once I had validated the output, I merged that into my main dataset on the ‘tweet_text’ column. I renamed the additional column as 'tweets_per_post'. I added a conditional column 'content_type' which was a thread or singular post flag. Through this process, I was able to eliminate irrelevant information and highlight the significant details of our Twitter data.

## Data Analysis

### 1. What is our current content strategy?
![1 - content strategy](https://github.com/eoghenejakpor1/Social-Media-Content-Strategy-Project/assets/57187615/be97ed1e-0943-4470-beaf-3d9ae82aae33)
Our current content strategy revolves around a balanced approach, designed to engage our audience while maintaining consistency. On a daily basis, we are publishing between **1-2 single posts**, ensuring that our audience receives regular updates and insights. This frequency allows us to maintain a consistent presence and provide timely information. Additionally, to foster deeper discussions and dive into more comprehensive topics, we are crafting **3-5 threads each week**. These threads serve as platforms for more in-depth content, encouraging audience interaction and enhancing our brand's thought leadership in specific areas. By combining these two content formats, we aim to cater to varying audience preferences, ensuring we deliver value consistently while encouraging meaningful engagement.

### 2. How do our impressions evolve over time?
![2 - impressions over time](https://github.com/eoghenejakpor1/Social-Media-Content-Strategy-Project/assets/57187615/847044dd-e3de-43eb-9696-58681e06fa5a)
Diving into our data, I spotted some interesting shifts in how often our content is seen. In October, there was a big drop—**impressions fell by 43%**. This is a clear signal. It tells us that potentially our audiences’ preferences are changing or our content quality has dropped. It also further validates the need for this project as, if nothing were to change, I believe this trend would continue and tarnish our reputation as a brand.

### 3. Which type of content (threads or single posts) generates the highest engagement rate?
![3 - engagement rate](https://github.com/eoghenejakpor1/Social-Media-Content-Strategy-Project/assets/57187615/e672bf42-b9d0-418a-8ed7-7fbbf0efe889)
When it comes to engaging our audience, **threads are clearly the winners**. They generate **double the engagement** compared to single posts. Specifically, threads have an engagement rate of 5%, while single posts lag behind at just 3%. This means that for every interaction we get on a single post, we're seeing two interactions on a thread. So, if we aim to capture more attention and interaction from our audience, **focusing on threads will be more effective.**

### 4. Do impressions follow the same trend? Threads generate ~65% more Impressions vs Single Posts
![4 - impressions vs single posts](https://github.com/eoghenejakpor1/Social-Media-Content-Strategy-Project/assets/57187615/e00ee227-7952-491c-a3f1-69c379dc6ad3)
Looking at how many people see our content, **threads really stand out.** They get about **65% more views **than single posts do. To break it down, threads get 2.06 million views, while single posts only get 1.24 million. This shows that **threads are more effective in getting our content seen by a lot more people.**

### 5. Which type of content produces more user profile clicks and followers?

| Metric                     | Single Posts | Threads      | Verdict                                                |
|----------------------------|--------------|--------------|--------------------------------------------------------|
| Total User Profile Clicks   | 2435         | 3277         | Threads generate 35% more profile clicks vs Single Posts|
| Total Followers             | 276          | 483          | Threads attract 7X more followers than Single Posts    |

When it comes to getting people to click on our profiles and follow us, threads are the way to go. **Threads lead the pack,** getting **35% more profile clicks** than single posts. Specifically, single posts got 2,435 clicks, while threads scored 3,277. Even more impressive, threads also bring in more followers. Single posts added 276 new followers, but threads took the lead with 483 new followers. That's **75% more followers with threads** compared to single posts. So, if we want to grow our follower base and get more profile visits, focusing on threads seems to be the smart move.

## Results/Findings

Moving forward, it's evident that our thread posts are the driving force behind engagement and community growth, showcasing double the engagement rates compared to single posts. Furthermore, they've demonstrated a remarkable ability to amplify our reach, securing 65% more impressions and fostering a 75% increase in followership. Given these insights, o**ur immediate focus should be on enhancing our thread content strategy,** ensuring it remains robust and resonant with our audience's preferences.
