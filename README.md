
##### Tags: `React-Native` `Expo` `ios` `TikTok` `Parse` `Back4App` `JavaScript` `Python` 

`Source`: [hackmd](https://hackmd.io/iTm3xVF1QqqBcjUoR0uh1Q)

# TikTalk

Developing an app that displays TikTok's most popular sounds, creators, and a function that allows the user to match their audio input to a popular TikTok sound. This is an iOS that integrates web data extraction and a custom Parse backend server hosted on Back4App. 

## Table of Contents

- [TikTalk](#tiktalk)
  - [Table of Contents](#table-of-contents)
  - [Setup/Installation 🏗](#setupinstallation-)
  - [Yelp API](#yelp-api)
    - [Network](#network)
  - [Database](#database)
    - [Schema](#schema)
  - [Project Demo Features](#project-demo-features)
    - [API Data Presentation + Animations](#api-data-presentation--animations)
    - [User Auth + Group Chat](#user-auth--group-chat)
    - [MapKit + Image Upload](#mapkit--image-upload)
  - [Built With](#built-with)
  - [Authors](#authors)

## Setup/Installation 🏗


1. MacOS/Windows
2. Download and install [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/#mac-stable) or [Node](https://nodejs.org/en/download/)
3. After downloading your package manager, download and install [Expo](https://docs.expo.dev/get-started/installation/)
4. In the project directory, execute the following command `yarn` or `npm install` depending on which package manager you downloaded.
5. Finally, in the same directory, execute the command `expo run:ios` or `expo run:android` depending on the used simulator

## Parse API

We used [**Parse**](https://parseplatform.org/) (hosted on [**Back4app**](https://www.back4app.com/)) as our backend to handle the databases used to hold data regarding sounds and creators information.

[**Beautiful Soup**](https://pypi.org/project/beautifulsoup4/) was used to web scrape websites for data regarding the most popular tiktok sounds and creators.


### Network

- `POST` /search – retrieve businesses from a given search query in SF



## Database

We used [**mongoDB**](https://www.mongodb.com/) and [**Parse server**](https://parseplatform.org/), hosted on [**Back4App**](https://www.back4app.com/) to manage our data for the application. This helps students focus more on how iOS works connecting to a database and not get distracted or overloaded with learning backend development. 

### Schema

Below is the database schema for our simple Parse Databases.

**Sounds**

| Name       | Type   | Descrpition                          |
| ---------- | ------ | ------------------------------------ |
| rank   | int | popularity ranking |
| song_status_code | int | status code of song_url |
| title   | string | sound title               |
| artist | string | sound artist |
| views | string | views of sound |
| song_url | string | URL of sound to TikTok |
| image_url | string | URL of soud image |


**Creators**

| Name       | Type   | Descrpition                          |
| ---------- | ------ | ------------------------------------ |
| rank   | int | popularity ranking |
| user | string | creator username |
| nickname | string | creator nickname |
| location | string | creator location |
| followers | string | total following on TikTok |
| videos | string | total videos on TikTok |
| likes | string | total likes on TikTok|
| image_url | string | URL of soud image |

## Project Demo Features

Below are the following features that are capable for the app:


### Top TikTok Sounds Leaderboard

- Load data from Yelp API + Search Bar
	- <img src="https://i.imgur.com/SEyigmC.gif" height=400>

- Animations using [Lottie](https://airbnb.io/lottie/#/) and [SkeletonView](https://github.com/Juanpe/SkeletonView)
	- <img src="https://imgur.com/EJGYjhl.gif" height=400>

### Top TikTok Sounds Leaderboard

- Login/Logout
- Messaging/Chatting capabilities
- Save messages using [Parse Server](https://parseplatform.org/)
	- <img src="https://imgur.com/vhH5dkG.gif" height=400>

### Voice Recognition + Machine Learning

- Show business in Map
- Upload image to Map Pin
	- <img src="https://imgur.com/Npz2m1A.gif" height=400>


## Built With

- [Expo](https://www.yelp.com/fusion)
- [Parse Server](https://parseplatform.org/)
- [Beautiful Soup](https://parseplatform.org/)


## Authors

- **Efaz Ahmed** - [EfazAhmed](https://github.com/EfazAhmed)
  - Full-Sack Development
  - UI Design
  - MVC Architecture design + implementation
  - 


