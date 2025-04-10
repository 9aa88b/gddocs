# GS Value

GS values contain Information regarding certain aspects of the game

## GS Value structure

| key | value |
|:----|:------|
| 1 | Jumps |
| 2 | Attempts |
| 3 | Total Completed Official Levels |
| 4 | Total Completed Online Levels |
| 5 | Completed Demons |
| 6 | Total Stars |
| 7 | Total Completed MapPacks |
| 8 | Secret Coins Collected |
| 9 | Destroyed Players on the menu |
| 10 | Total Liked/Disliked levels |
| 11 | Total Rated Levels |
| 12 | User coins collected |
| 13 | Total Diamonds |
| 14 | current orbs |
| 15 | Completed Daily Levels |
| 16 | Shadow Shards |
| 17 | Poison Shards |
| 18 | Fire Shards |
| 19 | Ice Shards |
| 20 | Lava Shards |
| 21 | Demon Keys|
| 22 | Total Orbs Collected |
| 23 | Earth Shards |
| 24 | Blood Shards |
| 25 | Metal Shards |
| 26 | Light Shards |
| 27 | Soul Shards |
| 28 | Moons |
| 29 | Diamond Shards |
| 30 | Fire Path Progress |
| 31 | Ice Path Progress |
| 32 | Poison Path Progress |
| 33 | Shadow Path Progress |
| 34 | Lava Path Progress |
| 35 | Earth Path Progress |
| 36 | Blood Path Progress |
| 37 | Metal Path Progress |
| 38 | Light Path Progress |
| 39 | Soul Path Progress |
| 40 | Amount of Completed Gauntlets |
| 41 | List Rewards |
| 42 | Completed Insane Levels |
| 43 | Wraith Chest Keys |
| unique_{LevelID}_{Coins Collected} | The Coins Collected on the Official Levels
| unique_secretB03 | Glubfub coin |
| unique_secret04 | Official level page secret coin |
| unique_secret06 | 'Sparky' coin |

## GS_completed

all completed levels

| Key | Value |
|:----|:------|
| `n_{levelID}`| beaten in normal Mode |
| `c_{levelID}` | Completed level|
| `d_{levelID}` | completed daily
| `g_{levelID}` | completed gauntlet
| `star_{levelID}` | Collected Stars|
| `dstar_{timelyID}` | Collected Stars for daily|
| `gstar_{levelID}` | Collected Stars for gauntlet |
| `demon_{levelID}` | Collected Demon |
| `ddemon_{timelyID}` | Collected Demon for weekly|
| `gdemon_{levelID}` | Collected Demon for gauntlet|

## GS_3

GS_3 contains info about all levels you have collected unverified coins for

| Structure |
|:----------|
|`{levelID}_{coins collected}`|

## GS_4

GS_4 contains info about all levels you have collected verified coins for

| Structure |
|:----------|
|`{levelID}_{coins collected}`|

## GS_5

GS_5 contains info about all the MapPacks you have beaten

| Structure |
|:----------|
|`<k>pack_{packID}</k><s>{stars Rewarded}</s>`|

## GS_6

GS_6 contains all the Purchased Icons on your account

| Structure |
|:----------|
|`<k>{ListingID}</k><s>{Price}</s>`|

## GS_7

GS_7 is the Highscore attempt of levels

| Structure |
|:----------|
|`<k>{levelID}</k><s>{percentage}</s>`|

## GS_8

Unused

## GS_9

GS_9 provides info about how many stars downloaded levels give to you

| Structure |
|:----------|
|`<k>{levelID}</k><s>{rewardedStars}</s>`|

## GS_10

GS_10 Contains the high score of All Official Levels you have played

| Structure |
|:----------|
|`<k>{ID}</k><s>{percentage}</s>`|

## GS_11

GS_11 Contains the reward data for the Timely Chests you have opened

| key | Description |
|:----|:------|
| `<k>{ChestType}_{ChestID}</k>` | reward Object |
| `k_{number}` | RewardItems -> the number corresponds to how many RewardItems the player will recieve |
| `kCEK` | The [encoder keys](/resources/client/gamesave/kCEK?id=kcek-8-and-9-structure) |

### Chest Types

| ID | type |
|:---|:-----|
| 1 | 4 hour chest |
| 2 | 24 hour chest |

## GS_12

GS_12 Contains the currently active [Quests](/resources/client/gamesave/quests)

## GS_14

The Diamond Rewards Collected from Challenges and Daily levels

| structure | type |Description |
|:----------|:------|:-----------|
|`{TypeID}{challenge/dailyID}` | int | The Number of Diamonds Earned | 

### TypeID's

| Types | Description |
|:------|:------------|
| c | Challenges/quests |
| d | daily levels |

## GS_15

GS_15 Contains the upcoming [Quests](/resources/client/gamesave/quests)

## GS_16

GS_16 contains the High Scores for daily and weekly demons

| Structure |
|:----------|
|`<k>{TimelyID}</k><s>{percentage}</s>`|

## GS_17

GS_17 contains the Stars rewarded for daily and weekly demons

| Structure |
|:----------|
|`<k>{TimelyID}</k><s>{Stars}</s>`|

## GS_18

GS_18 contains the High Scores for Gauntlet Levels

| Structure |
|:----------|
|`<k>{levelID}</k><s>{percentage}</s>`|

## GS_19

GS_19 Contains the reward data for the Treasure room chests you have opened

| key | Description |
|:----|:------|
| `<k>{ChestID}</k>` | reward Object |
| `k_{number}` | RewardItems -> the number corresponds to how many RewardItems the player will recieve |
| `kCEK` | The [encoder keys](/resources/client/gamesave/kCEK?id=kcek-8-and-9-structure) |

## GS_20

GS_20 seems to be the total amount of Demon Keys you have had over your accounts lifespan

## GS_21

GS_21 Contains the reward data for the gauntlets you have completed

| key | Description |
|:----|:------|
| `g_{GauntletID}` | the gauntlet number |
| `00{ChestID}` | ChestIDs for Reward Chests |
| `k_{number}` | RewardItems -> the number corresponds to how many RewardItems the player will recieve |
| `kCEK` | The [encoder keys](/resources/client/gamesave/kCEK?id=kcek-8-and-9-structure) |

### Chest IDs

| ID | how to get |
|:----|:------|
| 0001 | Beat the Challenge |
| 0002 | Release the Demon Guardian |
| 0003 | Chamber of Time Chest|
| 0004 | Treasure Room 50 key Chest|
| 0005 | Treasure Room 100 Key Chest|
| 0006 | Treasure Room 200 Key Chest|
| 0007 | YouTube Chest |
| 0008 | Twitter Chest |
| 0009 | Facebook Chest |
| 0010 | Twitch Chest |
| 0011 | Discord Chest |
| 0022 | Zolguroth Chest (repeatedly poke Shopkeeper and return to shop) |
| 0023 | Help Button Chest |
| 0024 | Reddit Chest |

All chests between 0012 and 0021 are Ad Chests from the free versions of the game.


## GS_22

GS_22 Contains reward data for all of the ad chests from Geometry Dash world

| Key | Value |
|:----|:------|
| `{unix Timestamp}` | orbs |

## GS_23

GS_23 contains the High Scores for daily and weekly demons

| Structure |
|:----------|
|`<k>{TimelyID}</k><s>{percentage}</s>`|

## GS_24

GS_24 contains the High Scores for Gauntlet Levels

| Structure |
|:----------|
|`<k>{levelID}</k><s>{percentage}</s>`|

## GS_25

GS_25 Contains the reward data for every weekly demon you have completed

| key | Description |
|:----|:------|
| `d100{number}` | The Timely ID of the weekly Demon you have beaten |
| `k_{number}` | RewardItems -> the number corresponds to how many RewardItems the player will recieve |
| `kCEK` | The [encoder keys](/resources/client/gamesave/kCEK?id=kcek-8-and-9-structure) |

## GS_26

GS_26 is your currently active path. The value is the same as the path key in GS_value. Contary to most GS's, it's an integer value and not a dictionary.

| Structure |
|:----------|
| `<k>GS_26</k><i>{path}</i>` |

## GS_27

GS_27 contains the List Rewards you have acquired

| Structure |
|:----------|
|`<k>lr_{listID}</k><s>{diamonds}</s>`|

## GS_28

GS_28 contains your enabled items. All of them are strings (although they act as booleans). The animations (18-20) are set to 1 after doing.. something? even if not unlocked. The music unlocker is set to 1 by default as soon as you start the game. The music customize is set to 1 permanently when you unlock it.

| Key   | Description          |
|:------|:---------------------|
| 17_12 | Music Unlocker       |
| 18_12 | Slow Robot Walk      |
| 19_12 | Fast Robot Run       |
| 20_12 | Spider Naruto Run    |
| 21_12 | Music Customizer     |

## GS_29

GS_29 is unknown but is related to trying to fix some path bug. Contary to most GS's, it's a boolean value and not a dictionary.

| Structure |
|:----------|
| `<k>GS_29</k><t />` |
