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

This analysis was performed using Python and a powerful group of Python libraries including Pandas, Matplotlib, NLTK, ImageAI, WordCloud, and more.

The analysis were performed in a Jupyter Notebook (particularly, in Jupyter Lab).

## Data Source

The data used in this analysis was retrieved from YouTube API. A script was written to run each day throughout 2019 and fetch data from YouTube API about the trending videos of that day (for many countries). The script would then process the data received from YouTube and store them in text files.

The script is not my work. It can be found on Github: [ Trending-YouTube-Scraper](https://github.com/mitchelljy/Trending-YouTube-Scraper).

I put the script on a AWS EC2 instance and scheduled it—using Crontab—to run every day at a specific time.

After 2019 ended, I connected to the AWS instance using FileZilla application and downloaded all the data produced by the script. There was a file for each country for each day of 2019. I fetched data for 20 countries. So as a result, I downloaded 7,300 files.

To perform the analysis, I needed to process the data in order to merge the files for each country into a single CSV file.

## Data Size and Description

**In this post, United-States trending videos will be analyzed**, which constitute a total of 72,994 videos. YouTube usually place 200 videos in the trending list each day which would mean that we should have 73,000 (365 x 200) videos. We have 72,994. This is probably because on a few days, the number of Trending videos was slightly less than 200. 

So **we have data on 72,994 trending videos to analyze**. On YouTube, the same video might appear on the trending list for many days. This means that the 72,994 videos are not unique videos. In fact, among the 72,994 videos, we have **11,177 unique videos**. 

In other words, 11,177 videos showed on the trending list throughout 2019. Some of them might have stayed on the list for 10 days, some for 20 days, etc. We will see later in the analysis more info about this.

The following table shows an example of the data that we have for each video:

![Screen Shot 2020-05-01 at 10.03.48 PM](/Users/ammar/Downloads/Screen Shot 2020-05-01 at 10.03.48 PM.png)

As we can see, we have the ID of the video which is a unique value for the video across YouTube (No two videos have the same ID). We also have the title of the video, its publishing date and time, the channel that published it, its category, and its description and tags. We also have the number of the views, likes, dislikes, and comments of the video. There are also a few more data shown in the table. 

We can see that there is a field named "trending_date". This field specifies the date on which this video was trending. As we said earlier, the same video might appear on the trending-videos list for more than one day. This means that we might find another record in the data for the same video ID but with different "trending_date" and maybe different number of views, comments, likes, etc. (because those numbers are likely to increase from one day to another).