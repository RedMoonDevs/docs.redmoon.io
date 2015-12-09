ClanSeeker
==========

## 1. Quick Introduction
### What is ClanSeeker?
Basically, ClanSeeker is a [WebAPI](https://en.wikipedia.org/API) that permits its users to fetch [**Clash of Clans**](https://clashofclans.com/) data from the Supercell's servers.
It can vary from PlayerData to ClanDetails, going through ClanSearch _et catera_.

### In what cases can we use it?
You can use it mainly for your clan's website. Or as a management-app system for a clan family. Who knows?

## 2. Getting Started
### Protocol
The protocol used by ClanSeeker is simple. API Calls are done with a simple GET request _(HTTP/1+)_ and the arguments are passed in the same way.
This is an example of how the protocol is designed: ```http://api.clanseeker.co/command/?arg1=value&arg2=value```.

#### Arguments
The arguments have, in a certain way, types.
Name | Possible Values | Comments
--- | --- | ---
int | From Integer.MIN_VALUE to Integer.MAX_VALUE | Not used.
long |  From Long.MIN_VALUE to Long.MAX_VALUE | Used for IDs and such.
String | Alpha characters, encoded in UTF-18 |
boolean | true/false |

### Commands
Name | Raw Name | Usage
--- | --- | ---
[Version](#!cs/version.md) | `version` | Gets the version of the running API.
[PlayerVillage](#!cs/player_village.md) | `player_village` | Gets a player's data.
[ClanSearch](#!cs/clan_search.md) | `clan_search` | Search a clan.
[ClanDetails](#!cs/clan_details.md) | `clan_details` | Gets the clan's details.

## ClanSeeker API servers

ClanSeeker is available for download to run on your own servers. Here is a list of trusted API servers if you don't want to host your own:

API URL | Web Interface | Notes
--- | --- | ---
`api.clanseeker.co` | [clanseeker.co](http://clanseeker.co) | The official API, run by RedMoon

### Running your own server

To run your own server, simply download and extract ClanSeeker, `cd` to the directory it is contained in, and run:

```
java -jar ClanSeeker_Server.jar
```

Before it works, you will need to configure the server. You can do this by editing [`config.json`](cs/config_json.md).

Relevant documentation:

  * [Config.json](cs/config_json.md)

## 3. License
Any project and/or website using this API should be reported to BananaEater (Skype: `benjamin.collord`).
