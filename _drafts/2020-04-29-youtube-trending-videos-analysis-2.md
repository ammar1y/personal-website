# Analyzing YouTube Trending Videos in 2019

Around 1.5 years ago, a few months after entering the data-science field, I did an analysis of YouTube trending videos in US. That analysis was performed on trending videos of some months in 2017 and 2018; 40,000 videos were analyzed. The analysis attracted some interest on Kaggle and Reddit; I also received some emails praising the work done. That was 1.5 years age.

Today, I present an improved and expanded version of that analysis. This analysis is more advanced and contains new and interesting elements. Also, this time the analysis will cover more countries, not just the US.

## What are YouTube Trending Videos?

YouTube is the most popular and most used video platfrom in the world today. YouTube has [a list of **trending videos**](https://www.youtube.com/feed/trending). I'll quote the description of trending videos from [YouTube itself](https://support.google.com/youtube/answer/7239739?hl=en):

> Trending helps viewers see what’s happening on YouTube and in the world. Trending aims to surface videos that a wide range of viewers would find interesting. Some trends are predictable, like a new song from a popular artist or a new movie trailer. Others are surprising, like a viral video. Trending isn't personalized and displays the same list of trending videos in each country to all users.
>
> The list of trending videos is updated roughly every 15 minutes. With each update, videos may move up, down, or stay in the same position in the list.

## Goals of the Analysis

The main goal of the analysis is to find interesting facts and patterns by exploring the data and by using effective visualizations.

The analysis aims to explore the following:

- Among all the trending videos in 2019, which videos have the maximum view count (top 7 videos)?
- What is the average/minimum/maximum view count for 2019's trending videos?
- Which videos appeared on the trending list the most (because some videos might appear on the trending list for more than one day)? 
- What percentage of trending videos have their titles fully uppercase?
- How many videos contain 1 uppercase word? 2 uppercase words? 3 uppercase words?...
- XXpercentage of title-case titles
- What are the most common words in the titles of trending videos?
- What are the most common symbols in the titles of trending videos?
- What are the most common emojis in the titles of trending videos?
- What are the most common bigrams (2 consecutive words) in the titles of trending videos?
- What are the title lengths of the trending videos? What is the average/minimum/maximum title length? Which videos have the minimum title length?
- Which channels have more trending videos than others (top 10 channels)?
- What are the top categories of trending videos? Are "Entertainment" videos more trending than "Gaming" videos for example?
- At what times of the day were the trending videos published? Were more trending videos published in day hours or night hours? XXUTC
- How many views/comments/likes trending videos have when first appearing on the trending list?
- Trending videos that have their dislikes more than their likes when first appearing on the trending list
- How many days are between publishing a video and its first appearance on the trending list?
- How long are the descriptions/tags of trending videos?
- What are the most common words in the descriptions/tags of trending videos?
- What are the most used colors in the thumbnails of trending videos? (Analysis of the thumbnails of all trending videos)
- How hashtags are used in trending-videos descriptions?
- What are the most common objects in the thumbnails of trending videos? (Running AI object detection algorithm on all thumbnails)

## Tools Used



 Here we will use **Python** with some packages like **Pandas** and **Matplotlib** to analyze a dataset that was collected over 205 days. For each of those days, the dataset contains data about the trending videos of that day. It contains data about **more than `40,000` trending videos**. We will analyze this data to get insights into YouTube trending videos, to see what is common between these videos. Those insights might also be used by people who want to increase popularity of their videos on YouTube.