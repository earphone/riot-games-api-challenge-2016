# Random Mastery Game

This is the entry for the April 2016 Riot Games API Challenge dealing with Champion Mastery.

I decided to create a simple HTML multiple choice game using data that was pulled from random Summoners. Some help was given by Breao in fleshing out the idea as well as some modification to my original game code.

#### You can go the game's main page [HERE] (http://earphone.github.io/maingame.html)

## Data

In order to get the best representation of our peers and fellow Summoners, there was only one real way that was decided on, random. I do not know what it is about randomness but I always seem to be coming back to this. Even in the last API challenge, we work with randomness.

The randomness this time was accomplished with the help of an HTML I wrote called randomSummonerGenerator. The final version of this randomly generated an 8-digit number, which then called an API function to see if it was a real person and then we kept the data for Summoner's who were worthy and dedicated to the game (level 30).

In theory this was easy and straight-forward, in practice however, it was a different story completely. I kept running into Summoner's that seemed to be generated randomly or as placeholders (somehow they all started with "IS1"). After accomodating for this anomoly, I noticed that only about 1/3 of the actual Summoner's Ids that I was grabbing actually were level 30. Even less than that were Summoners that had played the game recently enough to have the data for Champion Mastery. All in all, I was able to grab data from about 5000 Summoners and use it as a basis for my game's questions. 

The data.xmlx that is shown in this repo is a sample of what I have done because my bandwidth kept timing out when I was trying to upload the original data sheet.

## Game

Once I had the data that I wanted, writing the game was the easy part. I encountered very few erros on this part and actually went a lot smoother than I had anticipated.

Please excuse the very crude and basic layout. I am still working on learning HTML as well as the Javascript needed to make everything work. That being said, I am proud for how it has turned out. 

#### Resources Used
* [RIOT Games API](https://developer.riotgames.com/api/methods)
* [ddragon](http://ddragon.leagueoflegends.com/tool/)
* [Github](https://github.com/)
* [Brackets](http://brackets.io/)