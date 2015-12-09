# Config.json (ClanSeeker)

## Example config

```
{
  "server": {
    "path": "/",
    "port": 8338
  },
  "game": {
    "clientsWorking": 2,
    "clients": [
      {"id": 209843,
      "token": "qrt9sj83ujaald899snzth2dg344bweea",
      "name": "RedMoon"}
    ],
    "gameVersion": {
      "version": "7.200.22",
      "sha": "b07b1997df077c85b4863d965aa9f7eb20a0831c"
    },
    "timeout": 5000
  }
}
```

## Configuration parameters

### `server` block

```
"server": {
  "path": "/",
  "port": 8338
},
```

`path`: A path for your server to be hosted on, `/` by default. If you did `/api` for example, your API would be located at `http://IP:PORT/api/...`.

`port`: The port your API will be accessed from, `8338` by default. Changing this to `80` would allow you to not have to type a port in your requests, but it would prevent other webservers from running.

### `game` block

```
"game": {
  "clientsWorking": 2,
  "clients": [
    {"id": 209843,
    "token": "qrt9sj83ujaald899snzth2dg344bweea",
    "name": "RedMoon"}
  ],
  "gameVersion": {
    "version": "7.200.22",
    "sha": "b07b1997df077c85b4863d965aa9f7eb20a0831c"
  },
  ```

`clientsWorking`: How many clients should be actively working. This should be set to how many clients you want actively running for calls, with the rest acting as backups Set this to a **minimum** of 1. We recommend setting this to 1 or 2 less than the amount of client accounts you have to ensure you have a backup account ready.

`clients`: Configuration for client accounts, to login to the Clash of Clans servers. Clients is set in the following manner:
```
"clients": [
  {"id": USER-ID,
  "token": "USER-TOKEN",
  "name": "USER-NAME"},
  {"id": USER-ID,
  "token": "USER-TOKEN",
  "name": "USER-NAME"},
  {"id": USER-ID,
  "token": "USER-TOKEN",
  "name": "USER-NAME"}
  . . .
],
```
  You can add more {"id"...} brackets, as many as you want for the amounts of accounts you have credentials to.
* `id`: <!-- ALEX WRITE THESE -->
* `token`
* `name`

`gameVersion`: Game configuration. Replace `version` and `sha` with the current Clash of Clans version information.

### Miscellaneous

`timeout`: The amount, in milliseconds of time it takes before the API drops a request.
