Meta Data Analysis – Instagram User Engagement & Marketing Strategy
Project Overview
This project analyzes Instagram user activity and engagement data to help Meta's Marketing Team develop targeted strategies to improve user engagement, retention, and acquisition.

Using SQL, the project explores patterns across user accounts, photo posts, likes, comments, follows, and hashtags. The findings are translated into practical recommendations for encouraging inactive users to participate and helping active creators sustain and grow their engagement.
Business Problem
Meta wants to better understand how people use Instagram and identify the behaviors that distinguish active users from inactive users. The goal of this analysis is to uncover meaningful patterns in the platform's data and recommend sustainable, data-driven marketing actions.
Project Objectives
- Examine the database for duplicate and missing values.
- Measure user activity through posts, likes, and comments.
- Calculate average engagement per post and compare creator performance.
- Identify users with the highest follower and following counts.
- Find users who have never posted or liked content.
- Analyze hashtag usage and engagement by content theme.
- Review monthly activity, signup patterns, posting times, and follow-back behavior.
- Segment users based on their posting, engagement, and social activity.
- Develop marketing recommendations for active and inactive users.
Dataset
The project uses seven interconnected tables from the Instagram-style ig_clone database:
Table	Description
users	User accounts, usernames, and signup timestamps
photos	Photos uploaded by users
comments	Comments made by users on photos
likes	Likes given by users to photos
follows	Relationships between followers and followed users
tags	Hashtag categories
photo_tags	Mapping between photos and tags


The project documentation reports that the supplied tables contain no duplicate or missing/null values. The analysis primarily focuses on photo-based content; the dataset does not provide video or Reels records for a direct format comparison.
Tools & Technologies
- SQL / MySQL – Data querying, exploration, aggregation, and analysis
- MySQL Workbench – SQL development and query execution
- Microsoft PowerPoint – Presentation of findings and marketing recommendations
SQL Techniques Used
The SQL analysis applies:
- INNER JOIN and LEFT JOIN
- Subqueries and correlated NOT EXISTS queries
- Common Table Expressions (CTEs)
- Aggregate functions such as COUNT, SUM, and ROUND
- Conditional logic using CASE
- Window functions and ranking concepts
- Date and time functions, including DATE_FORMAT, DATEDIFF, and HOUR
- GROUP BY, HAVING, sorting, and filtering
Key Analysis Areas
1. Platform Overview
The project examines the total number of users, photos, likes, and comments to establish a baseline view of platform activity.
2. User Activity & Engagement
It calculates user-level posting, liking, and commenting activity, along with average engagement per post. It also identifies users who have never posted or liked a photo.
3. Creator & Follower Analysis
The analysis ranks users by photo volume, engagement received, followers, and following counts. It also explores follow-back behavior.
4. Hashtag & Content Theme Analysis
Hashtag usage is evaluated by post count and engagement. This helps identify popular themes that can inform content curation and more relevant campaign ideas.
5. Time-Based Analysis
The SQL queries examine monthly posting and engagement trends, signup patterns, user tenure, and the hours in which photos are posted.
6. User Segmentation
The project develops behavior-based segments, including:
- Influencer
- Active Creator
- Passive Engager
- At-Risk
- Content Consumer
- Casual User
These segments can help tailor activation, retention, and creator-support initiatives.
Key Findings
The accompanying project presentation reports the following results from the supplied dataset:
Metric	Finding
Total users	100
Total photos	257
Total likes	8,782
Total comments	7,488
Hashtag categories	21
Users who posted at least once	74
Users who never posted	26
Average likes per photo	34.17
Average comments per photo	29.14
Average photos per active user	3.47


Additional observations highlighted in the presentation:
- Approximately 26% of the users had never uploaded a photo.
- The presentation reports roughly 63 combined likes and comments per photo on average.
- The smile hashtag was the most frequently used category, with 59 uses.
- The most-followed user and the user following the most accounts were different users.
- Approximately 23% of users had never commented.
These figures describe the dataset analyzed in this project and should not be interpreted as current Instagram-wide statistics.
Business Recommendations
Based on the analysis and the accompanying presentation, the project proposes:
For Active Users & Creators
- Introduce monthly leaderboards that recognize consistent posting and engagement.
- Give high-performing creators additional in-app visibility.
- Explore creator spotlights and brand-collaboration opportunities.
- Build community initiatives and events that encourage creators to remain active.
For Inactive Users
- Use targeted outreach to encourage first-time posting.
- Demonstrate the benefits of participating and connecting with other users.
- Use creator stories and peer examples to make participation more approachable.
- Include inactive users in platform-wide engagement campaigns.
For Content & Marketing
- Use popular hashtag themes to inform relevant campaign concepts.
- Tailor campaign messages to different user activity segments.
- Encourage a wider range of user-generated content themes.
- Monitor engagement and retention measures to evaluate campaign performance.
Project Deliverables
- SQL script containing exploratory, objective, and business-focused analysis queries.
- Project documentation describing the problem statement, questions, SQL approach, and explanations.
- Storytelling presentation summarizing dataset insights, diagnosis, and recommendations.
Repository Structure
Project-Meta-Data-Analysis/
│
├── Meta_data_analysis.sql
├── META_DATA_ANALYSIS_aligned.docx
├── Meta_Data_Analysis_Storytelling.pptx
└── README.md
File names in your repository may differ slightly from the names shown above.
How to Run the SQL Analysis
1. Install and open MySQL Workbench (or another compatible MySQL client).
2. Create or load the ig_clone database and its seven tables.
3. Import the dataset used for the project.
4. Open Meta_data_analysis.sql.
5. Execute the queries section by section to explore platform metrics, user behavior, engagement, hashtags, and time-based patterns.
6. Review the project document and presentation for the interpretation of results and proposed marketing actions.
Note: The SQL script begins with USE ig_clone;, so the database must exist and be populated before running the queries.

Project Outcome
This project demonstrates how relational data and SQL analysis can be used to understand social-platform behavior, identify inactive and high-performing user groups, evaluate engagement patterns, and translate findings into actionable marketing recommendations. It combines technical querying with business-oriented interpretation and storytelling.
Author: Pallerlamudi Srikanth
