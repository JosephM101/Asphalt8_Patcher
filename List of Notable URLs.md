# List of notable URLs
- `http://vgold-eur.gameloft.com:20000/1781:53961:3.2.0r:windows:windows8/locate?service=auth` -> returns "eur-janus.gameloft.com:443" (as of 6/22/2023)
  * `3.2.0r`: Looks like the game is sending its version (tested on Asphalt 8 version 3.2.0r)
  * `service`: Found values `auth`, `storage`, `message` and `asset` being specified in packet captures. Each value results in different URLs, all resolving to IP "208.71.185.241". This likely means there is a reverse proxy present.

- `http://201205igp.gameloft.com/redir/rewards.php?action=retrieveitems&game_code=[game_code]&lang=EN&game_ver=3.2.0r&d=[d]
- `http://a314.gameloft.com/un/index.hhh?event=init`
