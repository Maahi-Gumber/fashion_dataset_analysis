# fashion_dataset_analysis
This notebook performs a time series analysis of MESHKI’s Instagram videos and reels, modeling engagement over time and showing that the main spike in performance coincides with a high‑profile celebrity collaboration.


Meshki Instagram Time Series Analysis
This project analyzes the time series evolution of MESHKI’s Instagram video and reel performance to understand how their social media presence changes over time and how major collaborations impact engagement. It uses post‑level metrics (views, plays, likes, comments) and timestamps to model engagement dynamics and identify periods of significant growth.
​

Project Goals
Build a cleaned, time‑indexed dataset of MESHKI Instagram posts, focusing on videos and reels.
​

Compute engagement and weighted engagement rate from likes, comments, and video plays/views.
​

Perform time series modeling (Prophet) to capture trends, weekly/seasonal patterns, and forecast engagement.
​

Detect and visualize engagement spikes and relate them to key marketing events such as a high‑profile celebrity collaboration.
​

Evaluate whether the major upward shift in engagement coincides primarily with that celebrity partnership window.
​

Data and Features
The notebook works from a large exported Instagram dataset (meshki_dataset.csv) with over 1,600 columns, including:
​

Post metadata: caption text, type (Video, Sidecar, etc.), tagged users, URLs.
​

Engagement metrics: commentsCount, likesCount, videoPlayCount, videoViewCount.
​

Time information: ISO timestamps converted to timezone‑aware datetimes (Australia/Sydney) for time series work.
​

Derived features: selected engagement columns and a standardized / weighted engagement rate used for modeling.
