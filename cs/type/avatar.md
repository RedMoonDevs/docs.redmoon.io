Avatar
======

## Components
Component | Type | Details
--- | --- | ---
`userId` | long | The ID of the Player (aka. PlayerID)
`currentHomeId` | long | The other ID
`clanId` | long | The Clan's ID _(if it has any)_
`clanName` | String | The Clan's name _(if it has any)_
`clanBadge` | int | The Clan's badge _(if it has any)_
`clanRole` | ClanRole (String) | The Player's role in the Clan _(if it has any)_
`clanWar` | int |
`userToken` | String | The Player's token, _(hidden)_
`fbid` | String | The Player's Facebook ID
`gcid` | String | The Player's GameCenter ID
`numberLogin` | int | How many times has the player logged in? _(hidden)_
`secondsLogin` | int | Since when did the Player **not** log in? _(hidden)_
`league` | League (String) | The League
`townHallLevel` | int | The TownHall Level of the Player
`userName` | String | The Player's username
`level` | int | The Player's level
`XP` | int | The Player's XP (experience)
`gems` | int | The Player's Gems count, _(hidden)_
`freeGems` | int | The Player's FreeGems count, _(hidden)_
`attackRating` | int | The Player's AttackRating
`attackKFactor` | int | The Player's AttackKFactor
`trophies` | int | The Player's trophy count
`attackWinCount` | int | The Player's won attack count, _(hidden)_
`attackLoseCount` | int | The Player's lost attack count, _(hidden)_
`defenseWinCount` | int | The Player's won defense count, _(hidden)_
`defenseLoseCount` | int | The Player's lost defense count, _(hidden)_
`nameChosenByUser` | boolean | Was the name chosen by the Player?
`nameChanged` | int | How many name changes left?
`boughtGems` | int | The number of Gems bought by the Player
`resourcesCapList` | DataSlot[] | The capacity of the Player's Resources
`resourcesList` | DataSlot[] | The Player's Resources
`troopsCount` | DataSlot[] | The Troops count
`spellsCount` | DataSlot[] | The Spells count
`troopsLevels` | DataSlot[] | The Troops' levels
`spellsLevels` | DataSlot[] | The Spells' levels
`heroesLevels` | DataSlot[] | The Heroes' levels
`heroesHealth` | DataSlot[] | The Heroes' health
`heroesState` | DataSlot[] | The Heroes' state
`allianceTroops` | UnitSlot[] | The Alliance Troops
`tutorialProgress` | DataReference[] | The progress of each Tutorial step
`achievements` | DataReference[] | The Achievements
`achievementsProgress` | DataSlot[] | The progress of each Achievements
`singlePlayerScore` | DataSlot[] | The score obtained in the SinglePlayer campaign
`singlePlayerGold` | DataSlot[] | The gold stolen fomr the SinglePlayer campaign 
`singlePlayerElixir` | DataSlot[] | The elixir stolen fomr the SinglePlayer campaign 
`givenTroops` | int | The count of donated troops
`receivedTroops` | int | The count of received troops

## See also...
- [Data](#!cs/type/data.md)
- [Village](#!cs/type/village.md)
- [Player](#!cs/type/player.md)