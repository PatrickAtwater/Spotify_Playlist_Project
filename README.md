![image](https://user-images.githubusercontent.com/83980785/129940315-3dee9770-4270-4bf9-b2b5-d2e28362291a.png)

# Spotify_Playlist_Project
A deep dive into the popular playlists on Spotify providing insights for the independent artist and how to earn income through these playlists.


# Summary
The Spotify Playlist project will take a look at the placement of songs by independent artists into popular playlists on Spotify. The most popular playlists will be analyzed with an attempt to answer whether or not strategic playlist placement can provide a viable source of income for the independent music artist. In addition, any common trends that are found amongst songs that are placed in the top playlists will be noted. The playlist data will be accessed through Spotify’s API. Expected challenges are going to be retrieving the correct data through the API into Python and cleaning it appropriately. In addition, tracking independent artists may or may not be possible depending on how the data is setup.
# Motivation

![image](https://user-images.githubusercontent.com/83980785/129940557-ce84ad96-2034-4d71-bc5c-36da7a342e27.png)

For this project, I am going to utilize Spotify’s API to gain insight into the world of playlist placement.  My intended audience is for independent musical artists who have suffered from the loss of live music and would like to learn how to dig in and start earning from playlist placement on Spotify.

# Data Questions
![image](https://user-images.githubusercontent.com/83980785/129940753-b82d70c7-d199-4b65-876b-0bd0a7c6c9f0.png)


### STRETCH GOALS (not currently available):
3. For a given artist, which playlists metadata match most closely to the artist's own catelog?
4. For the songs by independent artists, what was the trajectory of the song to being placed on the top playlist?
5.  Spotify typically pays between $0.003-0.005 per stream. How much are the artists on the top playlists earning and is that a viable way to make a living?


# Deliverables

![image](https://user-images.githubusercontent.com/83980785/129941038-e865b3e7-8a8b-4398-88c3-b9fdd38c0871.png)


## Data Acquisition

![image](https://user-images.githubusercontent.com/83980785/129941112-cb39b2d0-12b6-4670-829d-5894b94c001a.png)
### **Example of Python Code to pull Metadata for each song**
![image](https://user-images.githubusercontent.com/83980785/129941852-4aa30ca6-50e1-4024-85a6-d3e374facac9.png)

### **Example of Python Code to pull 100 songs for each genre**
![image](https://user-images.githubusercontent.com/83980785/129942114-4aaf7b1b-81a6-4d3c-8926-40db4384dd8d.png)
## Dashboards
### **Genre Dashboard**
### **Playlist Dashboard** [Click here to access Dashboard via web](https://app.powerbi.com/view?r=eyJrIjoiMTRhMTYyMGEtNmY2NC00ZmNhLWE4NzgtNWYzNDJiNWYyMGNkIiwidCI6IjEwMWRhNTg3LTE4NDMtNGY1Mi04YjhhLTE3YjA2OWM2NmQzMyIsImMiOjJ9)
![image](https://user-images.githubusercontent.com/83980785/129941580-1e550934-04f4-4b1a-b39d-b9477a2aa6c1.png)


# Key insights
Through accessing the provided Dashboard, we can pull insights such as follows: 
1. Most Popular Playlist: 
 * Playlist Name: Top 50 – Global
* Avg. Popularity: 89.5
* Notable Metadata points: 
    * There are zero instrumental tracks on this playlist
    * There is an above avg Danceability rating of .68 (.63 is overall rating)
    * 25% of the songs on this playlist are in C# or F#
2. The most popular song on Top 50 - Global:
* Track Title: Beggin'
* Artist: M√•neskin	
* Playlists Count: 13
* Popularity: 100 (out of 100)
* Key: B minor
* Tempo: 134 BPM
* Energy: 0.8 (out of 1)
* Danceability: 0.71 (out of 1)


## Data Sources

**IMPORTANT NOTE**<br />
**The Data for this project was compiled between 08-05-2021 & 08-12-2021 
and so  reflects a snapshot of the current offerings on Spotify. <br />
These lists would be curated over time and so would require 
updated data pulls to investigate current data and trends over time.**


* [Spotify Web API](https://developer.spotify.com/documentation/web-api/) <br />
	This API will be manipulated to procure data on the top playlists.


* [SpotiPy](https://github.com/plamere/spotipy#a-light-weight-python-library-for-the-spotify-web-api) - A light weight Python library for the Spotify Web API <br /> 
My hope is that implementing this library will save time in accessing the API and bringing the data into Python

## Articles and resources consulted:
o	[How To Get Music in Spotify Playlists – Digital Music News](https://www.digitalmusicnews.com/2017/06/21/spotify-playlists/) <br />
o	[Spotify Royalties Explained, In 3 Easy Diagrams…](https://www.digitalmusicnews.com/2013/12/04/spotifythreeeasy/)<br />
o	[Lance Allen DIY Spotify Success](https://artists.spotify.com/blog/lance-allen-and-the-new-secrets-of-diy-success)<br />

## Known Issues and Challenges
These are a few of challenges faced in this project and how I managed them.

1)	Accessing the API and learning how to retrieve the data through it. <br />I have never used an API before and so there will be an expected learning curve on how to do this. In order to work through this, I set aside plenty of time to explore API's calls in Jupyter notebooks. I also reached out to instructors and fellow classmates who have used API’s before.
2)	Once I accessed the API, will it be possible to access the data as I am intending?<br />
After performing exploratory Data Analysis using the API, it became apparent that that a key measure I was intending to acquire, track play counts, is not made available through an API call. <br />
Instead, Spotify API offers a measure called Popularity which is an algorhythm based measure between 1-100 based upon play counts as well as how recent those plays are. This suited my needs for the most part and so was used for the majority of the analysis.
