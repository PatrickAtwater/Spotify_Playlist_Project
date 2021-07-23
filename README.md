# Spotify_Playlist_Project
A deep dive into the popular playlists on Spotify providing insights for the independent artist and how to earn income through these playlists.


#Executive Summary
The Spotify Playlist project will take a look at the placement of songs by independent artists into popular playlists on Spotify. The most popular playlists will be analyzed with an attempt to answer whether or not strategic playlist placement can provide a viable source of income for the independent music artist. In addition, any common trends that are found amongst songs that are placed in the top playlists will be noted. The playlist data will be accessed through Spotify’s API. Expected challenges are going to be retrieving the correct data through the API into Python and cleaning it appropriately. In addition, tracking independent artists may or may not be possible depending on how the data is setup.
#Motivation
I have made my living as a freelance musician and educator for the past 15 years. I write my own music but mostly I perform other people’s music live. During the 15 years which I have worked as a professional musician, the music industry has changed dramatically. The old model of selling physical copies of your music has been replaced by digital forms of music. The trajectory of digital music has undergone multiple forms but has settled recently into streaming-based services. Listeners can access all of their favorite music via an app such as Spotify or Apple music without having to purchase the music at all, and it’s legal. Listeners pay for their music either via a monthly fee or by allowing advertisements. This works out wonderfully for the listener experience as you get access to all the music of the world for a relatively small amount of money compared to what you would spend if you purchased all of this music individually.

Now, how does this streaming model affect the creators of the music, the artists? In short, not very well. Whereas one used to sell an album for $10-15 each and best sellers would sell millions of copies, now best sellers are measured in number of streams and the PayScale is much lower, usually less than 1 penny per stream. The musical artists have spoken out against this pay structure but have been forced to turn to the live performance to turn a profit in their careers.
Enter 2020. What had become the breadwinner of the musical artist, live music, was suddenly shut down completely and for an extended amount of time. With live music removed as a viable option, at least temporarily, many artists turned back to digital music and streaming services to try to stay afloat and continue to build their careers.

Some folks were indeed able to find ways to make the streaming services work for them. This success, among others, was through the use of the many, many playlists on one streaming service, Spotify.

In 2018, Digital Music Alliance reported that 54% of listeners preferred to listen to playlists than albums and this reader projects that that number has only increased. Some of these top playlists have millions of monthly listens.  Therefore, some artists have had some financial success through some fortuitous placement onto widely popular playlists.

For this project, I am going to utilize Spotify’s API to gain insight into the world of playlist placement.  My intended audience is for independent musical artists who have suffered from the loss of live music and would like to learn how to dig in and start earning from playlist placement on Spotify.

#Data Questions
##MVP
There are 3 categories of playlist: Spotify curated, AI-curated, and user-curated.
Q1: What are the top earning playlists in each of these categories?
Q2: Of these top playlists, how many of the tracks are created/owned by independent artists?
##STRETCH
Q3: For the songs by independent artists, what was the trajectory of the song to being placed on the top playlist?
Q4: Spotify typically pays between $0.003-0.005 per stream. How much are the artists on the top playlists earning and is that a viable way to make a living?


#Minimum Viable Product (MVP)
The MVP for this project will be a dashboard either in Tableau or PowerBI and it will show the top playlists in performance (number of streams) over the last 18 months. In addition, it will sow which metadata categories are most common amongst these playlists. I would also like to highlight the way in which I utilized Python to access the Spotify API and clean the data.
Stretch goals:
 Include the ability to drill into songs by independent artists and track the history of those songs to their placement on these top playlists.
Include an income estimator where the estimated revenue from a given song can be calculated.
I would also like to include the use of SQL at some point in this project but that will become apparent as I dig into the data.

Schedule (through 08-20-2021)
1.	Get the Data (07-30-2021)
2.	Clean & Explore the Data (08-05-2021)
3.	Create Presentation of your Analysis (08-12-2021)
-	Should be a presentation, but could include a Jupyter Notebook or dashboard in Excel, Tableau, or PowerBI
4.	Internal demos (08-16-2021)
5.	Demo Day!! (08-20-2021)

Data Sources
•	Spotify Web API - https://developer.spotify.com/documentation/web-api/
o	This API will be manipulated to procure data on the top playlists from the last 18 months
•	SpotiPy - A light weight Python library for the Spotify Web API  - https://github.com/plamere/spotipy#a-light-weight-python-library-for-the-spotify-web-api
o	My hope is that implementing this library will save time in accessing the API and bringing the data into Python
•	Articles and resources consulted:
o	How To Get Music in Spotify Playlists – Digital Music News
o	Spotify Royalties Explained, In 3 Easy Diagrams…
o	Lance Allen DIY Spotify Success
Known Issues and Challenges
Explain any anticipated challenges with your project, and my plan for managing them
1)	Accessing the API and learning how to retrieve the data through it.
a)	I have never used an API before and so there will be an expected learning curve on how to do this.
b)	I plan to set aside plenty of time to work through this as well as reach out to instructors and fellow classmates who have used API’s before.
2)	Once I can access the API, will it be possible to access the data as I am intending?
a)	Until I can see the data, I am not certain that the kinds of insights I am hoping to gleam are accessible
i)	If this were the case, it may be necessary to alter the MVP so as to utilize the data available.
3)	I would like to use Tableau for this dashboard as I need more practice with the Tableau interface.
a)	There needs to be set aside plenty of time for digging deeper into Tableau.
b)	If Tableau is proving unfruitful, I will pivot to power BI with enough time to create a compelling PowerBI dashboard.
