# Tracking US Foreign Policy Interests
>Eric Gutiérrez, 10th February 2026.

### Motivation
Over the years, the topics that dominate global foreign policy discourses have shifted dramatically, reflecting the evolving challenges and strategic interests of each era. From the post-Cold War focus on traditional security to the modern urgency of climate change and supply chain resilience, the language of diplomacy is constantly changing. In this project, we quantify these shifts by tracking the importance of 200 foreign-affairs-related topics from 1998 to 2025. 

### Data & Methods
To derive the importance of each topic in any given year, we analyzed 700 reports published by foreign-affairs experts from the [Council on Foreign Relations](https://www.cfr.org/) between 1998 and 2025.

We began by lemmatizing the documents to standardize the vocabulary. We then generated a Term Frequency-Inverse Document Frequency (TF-IDF) matrix, which computes how distinct each term is within the corpus. It is important to stress that this metric does not measure volume (how many times a term appears), but rather salience (how central a term is to a specific document or time period).

To construct the time-series, we aggregated the TF-IDF scores by year, calculating the mean score across all documents published in that year. This reveals the average 'importance' of a topic annually, independent of the total number of reports published.

### Results
Our analysis generated a dataset containing importance scores for over 37,000 unique terms across 700 documents spanning the entire analysis period. To visualize the most significant shifts in interest, the interactive chart below displays the trends for the 200 most prominent topics.

### Conclusions
Ultimately, the trends identified in the dashboard above tell the story of a changing world. As new challenges emerge, the vocabulary of diplomacy will continue to adapt, serving as a real-time indicator of global priorities.