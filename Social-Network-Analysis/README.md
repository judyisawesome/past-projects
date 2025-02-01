
# Reddit Hyperlink Network Analysis

## Overview

This project leverages **Social Network Analysis (SNA)** to uncover hidden patterns and dynamics within Reddit's vast ecosystem of interconnected subreddits. By examining hyperlink interactions between subreddits from 2014 to 2017, we identified influential communities, explored cross-community engagement, and analyzed sentiment dynamics to better understand how information flows and how community interactions evolve on the platform.

## Objectives

- **Identify Influential Subreddits**: Pinpoint subreddits that serve as key hubs or bridges in the Reddit network using centrality metrics.
- **Explore Cross-Community Engagement**: Understand how different communities interact, form clusters, and disseminate content.
- **Analyze Sentiment Dynamics**: Study the tone of interactions to identify positive or negative clusters, providing insights into potential areas of toxicity or healthy engagement.

## Key Findings

### 🌐 **Network Structure and Influence**
- **Hubs and Bridges**: 
  - Subreddits like *AskReddit* emerged as central hubs, dominating multiple centrality metrics, while *subredditdrama* and *bestof* drove cross-community discussions.
  - *AskReddit*, *funny*, and *worldnews* acted as bridges, connecting otherwise disconnected communities and fostering diverse interactions.
- **Decentralization Trends**:
  - By 2017, a decline in centrality metrics suggested a decentralization trend as niche subreddits rose in prominence.

### 🔗 **Cross-Community Engagement**
- **Reciprocity and Clustering**:
  - Subreddits like *r/politics* and *r/The_Donald* exhibited strong bidirectional ties, especially around significant events like the 2016 U.S. Presidential Election.
  - Exponential Random Graph Models (ERGMs) revealed that while reciprocity played a significant role, overall subreddit interactions were sparse and hierarchical.
- **Content Dissemination**:
  - Subreddits like *r/news* served as critical bridges for distributing information, especially during high-activity periods like elections.

### 💬 **Sentiment Dynamics**
- **Complexity of Negative Sentiment**:
  - Posts with negative sentiment were significantly longer and used more complex language, indicating that users expressing dissatisfaction tend to elaborate more.
- **Centrality vs. Sentiment**:
  - A slight negative correlation was observed between subreddit centrality and sentiment, suggesting that highly connected subreddits often host more contentious discussions.

## Impact

- **Moderation Insights**: Our analysis equips moderators with actionable insights to foster healthier online communities by identifying potential areas of toxicity and promoting constructive engagement.
- **Platform Strategy**: Recommendations include leveraging central hubs for positive campaigns, tailoring moderation strategies to thematic clusters, and promoting cross-community dialogue to reduce echo chambers.
- **Business Applications**: Advertisers and content creators can optimize their strategies based on subreddit engagement patterns, reciprocity, and sentiment trends.

## Visualizations

- **Network Graphs**: Visualization of subreddit hyperlink interactions highlighted central hubs and isolated clusters, revealing patterns of content flow and community structure.
- **Sentiment Heatmaps**: Showed shifts in sentiment dynamics over time, linked to major events or controversies.

## Dataset

The dataset used in this project was sourced from the **[Stanford Network Analysis Project (SNAP)](https://snap.stanford.edu/data/soc-RedditHyperlinks.html)**.

## Technologies Used

- **R** for social network analysis and statistical modeling
- **Gephi** for network visualization
- **Exponential Random Graph Models (ERGMs)** for analyzing structural dependencies
- **Sentiment Analysis** techniques for understanding user interactions

## Team

- **Kira Luo**
- **Grace Xie**
- **Judy Zhu**
- **Sydney Li**

## References

For detailed code and methodologies, please refer to the files attached in the original submission.
